## Configuration

`$ git config --list`  Lista todas as configurações  

### Username Registration
`$ git config user.name` Mostra username registrado  
`$ git config user.name 'renan.brito'` Define username para o usuario o repositório local  
`$ git config --global user.name 'renan.brito'` Define userame global para o usuario de todos os repositórios  


### Editor Registration
`$ git config core.editor` Exibe o editor padrão  
`$ git config core.editor 'editor-name'` Altera o editor padrão  

### Save Credentials
`$ git config --global credential.helper cache --timeout=28800` Salva as credentiais por um tempo determinado  
`$ git config --global credential.helper cache` Salva as credencias permanentemente 

### Alias Registration
[https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases] (Git Alias Documentation)  
`$ git config alias.ALIAS COMMAND` Registra um alias local. ALIAS = Alias name, Command = Git Command   
`$ git config --global alias.ALIAS COMMAND` Registra um alias global  
`$ git config --get-regexp alias` Lista todos os alias  