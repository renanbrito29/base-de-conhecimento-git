# Branches

## Criar branches
`git branch branch_name` Cria uma nova branch  
`git checkout -b branch_name` Cria uma branch e altera  
`git push remote_repo:nova_remote_branch` Cria uma branch remota  

## Deletar branch
`git push remote_repo :remote_branch` Remove uma branch remota 
`git push -d 'remote_repo' 'remote_branch'` Deleta uma **BRANCH** remota 
`git branch -d branch_name` Deleta uma branch local sem novos commits  
`git branch -D branch_name` Deleta uma branch local com novos commits  

## Listar branches
`git branch -v` Lista todas as branches e seu ultimo commit *HEAD*    
`git branch -a` Lista todas as branches locais  
`git branch -r` Lista todas as branches remotas  
`git branch --no-merged` Lista todas branches não mergeadas  
`git branch --merged` Lista todas branches mergeadas  

`git checkout branch_name` Altera branch  