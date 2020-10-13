# Local Repository Commands

## Basics
`$ git init` Inicializa um repositório local  
`$ git clone 'repository_url'` Clona um repositório remoto  
`$ git status` Verifica o estado atual do repositório com base no **HEAD**  

## Adicionar e retirar arquivos da **STAGING AREA**  
`$ git add` Adiciona arquivos do working directory para staging area  
`$ git restore --staged` Retira arquivos da staging area para o working directory  
`$ git rm` Remove todos os arquivos do repositorio  
    **Parameters:** -f=force: Remove da stagging area; -r=diretorio'  

## Mover e renomear arquivos  
`$ git mv 'source.extersion' 'directory'` Move um arquivo  
`$ git mv 'source.extersion' 'new-source-name.extersion'` Renomeia um arquivo  

### Wildcards
`file.txt` `file1.txt file2.txt` `folder/` `*.txt` `file-*`

## Commit
`$ git commit -m 'message'` Realiza o commit movendo os arquivos da **INDEX** para o **HEAD**  
`$ git commit -am 'message'` Coloca o arquivo no stage em seguinda realiza o commit dos arquivos para o **HEAD**  
`$ git commit -amend -m 'message'` Altera a mensagem do ultimo commit 

## Desfazer mudanças

`git checkout file.txt` Descarta alterações que ainda não foram commitadas e que não estejam na **STAGING AREA** e volta para o HEAD    

`git reset file.txt` Remove o arquivo da **STAGING AREA**  

`git reset --mixed HEAD^` Remove todos os commits com base no HEAD e todos os arquivos voltam ao estado de **MODIFIED**  
`git reset --soft HEAD^` Remove todos os commits com base no HEAD e todos os arquivos voltam para a **STAGING AREA**    
`git reset --hard HEAD^` Remove todos os commits com base no HEAD e **WORKING DIRECTORY** é resetado com base no **HEAD**    

`git reset --mixed commit_hash` Move o HEAD para o commit especifico e todas as alterações voltam para o o estado de **MODIFIED**  
`git reset --soft commit_hash` Move o HEAD para o commit especifico e todas as alterações voltam para a **STAGING AREA**  
`git reset --hard commit_hash` Move o HEAD para o commit especifico e **WORKING DIRECTORY** é resetado com base no **HEAD**  

`git revert commit_hash`  Volta para um estado espefico, desfaz o commit passado por parametro e gera um commit de revert 