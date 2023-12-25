## Comandos Basicos Git

```bash
git init  #Inicia um novo repositorio git
```

```bash
git clone  #Copia um repositorio git
```

```bash
git status  #Informa o estado atual do repositorio
```

```bash
git add  #Adiciona um arquivo ao repositorio

git add .  #Adiciona todos os arquivos ao repositorio
```

```bash
git commit -m "Mensagem"  #Cria um commit com uma mensagem
```

```bash
git push  #Envia os commits para o repositorio remoto
```

```bash
git pull  #Baixa as alterações do repositorio remoto
```

```bash
git fetch  #Baixa as alterações do repositorio remoto
```

```bash
git branch  #Lista as branchs do repositorio
```

```bash
git checkout "Nome da branch"  #Muda para a branch informada
```

```bash
git merge "Nome da branch"  #Faz o a mesclagem da branch informada com a branch atual
```

## Comandos de Configuração

```bash
git config --global user.name "Nome"  #Configura o nome do usuario globalmente
```

```bash
git config --global user.email "Email"  #Configura o email do usuario globalmente
```

```bash
git config user.name "Nome"  #Configura o nome do usuario localmente
```

```bash
git config user.email "Email"  #Configura o email do usuario localmente
```

```bash
git config --global core.editor "Nome do editor"  #Configura o editor de texto globalmente
```

```bash
git config core.editor "Nome do editor"  #Configura o editor de texto localmente
```

```bash
git config --global alias."Nome do alias" "Comando"  #Cria um alias globalmente
```

## Comandos de Logs

```bash
git log  #Mostra o historico de commits
```

```bash
git log --decorate  #Mostra o historico de commits com informações adicionais
```

```bash
git log --author="Nome do autor"  #Mostra o historico de commits de um autor especifico
```

```bash
git shortlog  #Mostra o historico de commits de forma resumida
```

```bash
git shortlog -sn  #Mostra o historico de commits de forma resumida e ordenada por quantidade de commits
```

```bash
git log --graph  #Mostra o historico de commits de forma grafica
```

```bash
git show "Hash do commit"  #Mostra as alterações do commit informado
```

## Comandos de Diferenças

```bash
git diff  #Mostra as alterações feitas nos arquivos
```

```bash
git diff --name-only  #Mostra apenas os nomes dos arquivos alterados
```

```bash
git diff "Hash do commit"  #Mostra as alterações feitas no commit informado
```

```bash
git diff "Hash do commit" "Hash do commit"  #Mostra as alterações feitas entre os commits informados
```

```bash
git diff "Hash do commit" "Hash do commit" --name-only  #Mostra apenas os nomes dos arquivos alterados entre os commits informados
```

## Comandos de Desfazer

```bash
git checkout "Nome do arquivo"  #Desfaz as alterações feitas no arquivo informado
```

```bash
git reset HEAD "Nome do arquivo"  #Retira o arquivo informado da staged area
```

```bash
git reset --soft "Hash do commit"  #Retorna o repositorio ao estado do commit informado
```

```bash
git reset --mixed "Hash do commit"  #Retorna o repositorio ao estado do commit informado e retira os arquivos da staged area
```

```bash
git reset --hard "Hash do commit"  #Retorna o repositorio ao estado do commit informado e retira os arquivos da staged area e do working directory
```

## Comandos de Tags

```bash
git tag  #Lista as tags
```

```bash
git tag -a "Nome da tag" -m "Mensagem"  #Cria uma tag anotada
```

```bash
git tag -d "Nome da tag"  #Deleta a tag informada
```

```bash
git push origin "Nome da tag"  #Envia a tag informada para o repositorio remoto
```

```bash
git push origin --tags  #Envia todas as tags para o repositorio remoto
```

```bash
git checkout "Nome da tag"  #Muda para a tag informada
```

## Comandos de Branchs

```bash
git branch "Nome da branch"  #Cria uma nova branch
```

```bash
git branch -D "Nome da branch"  #Deleta a branch informada
```

```bash
git checkout -b "Nome da branch"  #Cria uma nova branch e muda para ela
```

```bash
git merge "Nome da branch"  #Faz o a mesclagem da branch informada com a branch atual
```

```bash
git rebase "Nome da branch"  #Faz o rebase da branch informada com a branch atual
```

## Comandos de Stash

```bash
git stash  #Guarda as alterações feitas no working directory
```

```bash
git stash list  #Lista os stashs
```

```bash
git stash apply  #Aplica o ultimo stash
```

```bash
git stash apply "Nome do stash"  #Aplica o stash informado
```

```bash
git stash drop  #Deleta o ultimo stash
```

```bash
git stash drop "Nome do stash"  #Deleta o stash informado
```

```bash
git stash pop  #Aplica o ultimo stash e o deleta
```

```bash
git stash pop "Nome do stash"  #Aplica o stash informado e o deleta
```

## Comandos de Rebase

```bash
git rebase "Nome da branch"  #Faz o rebase da branch informada com a branch atual
```

```bash
git rebase --continue  #Continua o rebase apos resolver os conflitos
```

```bash
git rebase --abort  #Cancela o rebase
```
