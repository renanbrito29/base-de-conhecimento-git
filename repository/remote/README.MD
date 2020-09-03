# Remote Repositoriy Commands

`$ git remote` Lista todos os repositórios remotos  
`$ git remote -v` Lista todos os repositórios remotos com a URL  
`$ git remote add 'remote_alias' 'repository_url'` Adiciona um apontamento para um repositório remoto  
`$ git remote set-url 'remote_alias' 'new_repository_url'` Altera a URL de um repositorio remoto  
`$ git remote show 'remote_alias'`  Exibe todos os objetos de um repositorio remoto  

### Enviar atualizações do **HEAD** para o repositorio remoto
`$ git push 'remote_repo' 'remote_branch'` Envia alterações para o repositório remoto na **BRANCH** destino  
`$ git push -u 'remote_repo' 'remote_branch'` Envia alterações e grava uma referencia para o repositorio e **BRANCH**  
  
### Receber e excutar atualizações

#### Atualização com git fetch + git merge
`$ git fetch remote_repo remote_branch` Atualiza o **HEAD** com base no repositório remoto na **BRANCH** origem  
`$ git merge FETCH_HEAD` Faz a junção do **HEAD** com o **WORKING DIRECTORY**  

#### Atualização com git pull
`$ git pull remote_repo remote_branch` Atualiza com **MERGE** o **WORKING DIRECTORY** com base no repositório remoto na **BRANCH** origem   
`$ git pull -u remote_repo remote_branch` Atualiza com **MERGE** o **WORKING DIRECTORY** com base no repositório remoto na **BRANCH** origem e cria uma referencia para o repositorio + **BRANCH**  
`$ git pull --rebase` Atualiza com **REBASE** o **WORKING DIRECTORY** com base no repositório remoto na **BRANCH** origem  
>*git pull é um atalho para os comandos git fetch + git merge*