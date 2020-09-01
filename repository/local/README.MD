# Local Repository Commands

## Basics
`$ git init` Inicializa um repositório local  
`$ git clone 'repository_url'` Clona um repositório remoto  
`$ git status` Verifica o estado atual do repositório com base no **HEAD**  

## Adicionar e retirar arquivos da **STAGING AREA**  
### Adicionando arquivo do WORKING DIRECTORY para o INDEX
`$ git add .` Adiciona todos os arquivos  
`$ git add 'file.txt'` Adiciona um arquivo unico  
`$ git add '*.txt'` Adiciona todos os arquivo com extensão .txt dentro do diretório files  
`$ git add 'file-*.txt'` Adiciona todos os arquivos que tem o nome file- e que tenha a extensão txt  

### Retirando arquivo do INDEX para o WORKING DIRECTORY  
`$ git restore --staged .` Retira todos os arquivos  
`$ git restore --staged 'file.txt'` Retira um arquivo unico  
`$ git restore --staged '*.txt'` Retira todos os arquivo com extensão .txt dentro do diretório files  
`$ git restore --staged 'file-*.txt'` Retira todos os arquivos que tem o nome file- e que tenha a extensão txt  

### Remover arquivos do Repositório
**Parameters:** -f = force: Remove da stagging area; -r = diretorio'
`$ git rm .` Remove todos os arquivos do repositorio  
`$ git rm 'file.txt'` Remove um arquivo unico do repositorio  
`$ git rm '*.txt'` Remove todos os arquivo com extensão .txt do repositorio  
`$ git rm 'file-*.txt'` Remove todos os arquivos que tem o nome file- e que tenha a extensão txt do repositorio  

### Mover e renomear arquivos  
`$ git mv 'source' 'destination'`Move um arquivo  
`$ git mv 'source' 'new_source_name'`Renomeia um arquivo  

### Commit
`$ git commit -m 'message'` Realiza o **COMMIT** movendo os arquivos da **INDEX** para o **HEAD**  
`$ git commit -am 'message'` Realiza o **ADD** em seguinda realiza o **COMMIT** dos arquivos para o **HEAD**  