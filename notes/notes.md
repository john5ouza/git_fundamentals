## **📌 Comandos Básicos**

### Navegação e arquivos:

```bash
ls               # lista arquivos
cd <diretório>   # muda de diretório
pwd              # mostra o diretório atual
cat <arquivo>    # mostra conteúdo do arquivo

```

### Git local:

```bash
git checkout <branch>       # muda de branch
git status                  # mostra alterações
git merge <branch>          # faz merge de outra branch
git diff                    # mostra diferenças
git commit -m "mensagem"    # cria commit
git checkout -b <nome>      # cria nova branch e muda para ela
git branch -D <nome>        # deleta branch local
git log                     # histórico de commits
git push                    # envia commits para o remoto
git remote add origin <url> # adiciona repositório remoto

```

---

## **⚙️ Fluxo de Trabalho Git Local**

1. Criar repositório:

```bash
git init

```

1. Editar/alterar arquivos
2. Verificar status:

```bash
git status

```

1. Adicionar arquivos ao stage:

```bash
git add <arquivo>

```

1. Commitar alterações:

```bash
git commit -m "mensagem"

```

1. Repetir passos 2 a 5 para continuar trabalhando

### Alternativa com branch:

```bash
git checkout -b <nova_branch>   # cria e muda para nova branch
# faz alterações
git status
git add <arquivos>
git commit -m "mensagem"
git checkout main
git merge <nova_branch>         # mescla alterações na main

```

---

## **🌐 Fluxo de Trabalho GitHub <> Local (Projeto Próprio ou da Empresa)**

1. Clonar repositório remoto:

```bash
git clone <url>

```

1. Criar e mudar para nova branch:

```bash
git checkout -b <nova_branch>

```

1. Fazer alterações nos arquivos
2. Verificar status, adicionar e commitar:

```bash
git status
git add <arquivos>
git commit -m "mensagem"

```

1. Enviar alterações para o remoto:

```bash
git push origin <nova_branch>

```

1. Abrir **Pull Request** no GitHub para a `main`
2. Após merge, excluir a branch remota:

```bash
git push origin --delete <nova_branch>

```

1. Voltar para main e deletar branch local:

```bash
git checkout main
git branch -D <nova_branch>

```

---

## **🌍 Fluxo de Trabalho GitHub <> Local (Projetos Open-Source)**

1. Fazer **fork** do projeto original
2. Clonar seu fork:

```bash
git clone <url_do_fork>

```

1. Criar e mudar para nova branch:

```bash
git checkout -b <nova_branch>

```

1. Fazer alterações, verificar status, adicionar e commitar:

```bash
git status
git add <arquivos>
git commit -m "mensagem"

```

1. Enviar para seu fork:

```bash
git push origin <nova_branch>

```

1. Abrir Pull Request do seu fork para a main do projeto original
2. Após merge, excluir branch remota:

```bash
git push origin --delete <nova_branch>

```

1. Voltar para main e deletar branch local:

```bash
git checkout main
git branch -D <nova_branch>

```