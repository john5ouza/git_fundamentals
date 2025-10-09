# GIT/GITHUB CLASSES AND FUNDAMENTALS

> Working on the fundamentals of Git and GitHub with examples and workflows and some updates.

### Fluxo de trabalho Git local
* git checkout -b
* cria ou atualiza arquivos
* git status
* git add arquivos
* git status
* git commit -m "minha mensagem"
* git checkout main

### Fluxo de trabalho GitHub <> Local (projeto próprio ou da sua empresa)
* git clone
* git checkout -b <nova_branch>
* alterações de arquivos
* git status
* git add arquivos
* git status
* git commit -m "nova mensagem"
* git push origin <nova_branch>
* abrir Pull request no GitHub para main
* excluir <nova_branch> origin
* git checkout main
* git branch -D <nova_branch>

### Fluxo de trabalho GitHub <> Local (projetos open-source)
* Fork do projeto para seu próprio github
* git clone
* git checkout -b <nova_branch>
* alterações de arquivos
* git status
* git add arquivos
* git status
* git commit -m "nova mensagem"
* git push origin <nova_branch>
* abrir Pull request no GitHub da branch fork para a main do projeto * original
* excluir <nova_branch> origin
* git checkout main
* git branch -D <nova_branch>