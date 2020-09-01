# Base de conhecimento GIT

## Instalacao GIT

[https://git-scm.com/](https://git-scm.com/)

* Linux: [https://git-scm.com/download/linux](https://git-scm.com/download/linux)  
* Mac: [https://git-scm.com/download/mac](https://git-scm.com/download/mac)  
* Windows: [https://git-scm.com/download/win](https://git-scm.com/download/win)  

## Web Repository Interface
* Github: [https://github.com/](https://github.com/)  
* Git Lab: [https://about.gitlab.com/](https://about.gitlab.com/)  
* Bit Bucket: [https://bitbucket.org/](https://bitbucket.org/)  

## CLI
* https://github.com/cli/cli  

## UI
* Git Kraken: [https://www.gitkraken.com/](https://www.gitkraken.com/)  
* Source Tree: [https://git-cola.github.io/](https://git-cola.github.io/)  
* Git Cola: [https://www.sourcetreeapp.com/](https://www.sourcetreeapp.com/)  

 ## Adicionando o nome da branch no terminal
1. Abrir o arquivo .bashrc
2. Adicionar a seguinte linha no final do arquivo  
`export PS1='\u@\h\[\033[01;34m\] \w\[\033[0;32m\]$(__git_ps1 " (%s)")\[\033[01;34m\]$\[\033[00m\] '`  
3. Reiniciar o terminal