# Repository Commands

## Basics
`$ git init` Inicializa um repositório local  
`$ git clone 'repository_url'` Clona um repositório remoto  
`$ git status` Verifica o estado atual do repositório com base no **HEAD**  

## Adicionar e retirar arquivos da **STAGING AREA**  
### Adicionando arquivo do WORKING DIRECTORY para o INDEX
`$ git add .` Adiciona todos os arquivos  
`$ git add 'file.txt'` Adiciona um arquivo unico  
`$ git add 'files/\*.txt'` Adiciona todos os arquivo com extensão .txt dentro do diretório files  
`$ git add 'file-*.txt'` Adiciona todos os arquivos que tem o nome file- e que tenha a extensão txt  

### Retirando arquivo do WORKING DIRECTORY para o INDEX
`$ git restore --staged .` Retira todos os arquivos  
`$ git restore --staged 'file.txt'` Retira um arquivo unico  
`$ git restore --staged 'files/\*.txt'` Retira todos os arquivo com extensão .txt dentro do diretório files  
`$ git restore --staged 'file-*.txt'` Retira todos os arquivos que tem o nome file- e que tenha a extensão txt  

### Remover arquivos do Repositório 
`$ git rm .` Remove todos os arquivos  
`$ git rm 'file.txt'` Remove um arquivo unico  
`$ git rm 'files/\*.txt'` Remove todos os arquivo com extensão .txt dentro do diretório files  
`$ git rm 'file-*.txt'` Remove todos os arquivos que tem o nome file- e que tenha a extensão txt  
`$ git rm -r 'directory_name` Remove um diretório    