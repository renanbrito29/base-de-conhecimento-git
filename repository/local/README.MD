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