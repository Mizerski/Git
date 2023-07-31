# Comandos Git 

## Configuração

1. `git config --global user.name "Seu Nome"` - Configura o nome do usuário globalmente.
2. `git config --global user.email "seu.email@example.com"` - Configura o email do usuário globalmente.
3. `git config --global core.editor "editor"` - Configura o editor de texto padrão para mensagens de commit.

## Iniciar um Repositório

1. `git init` - Inicializa um novo repositório Git local.
2. `git clone <URL>` - Clona um repositório remoto existente para o seu computador.

## Gerenciamento de Alterações

1. `git status` - Mostra o status das alterações no diretório de trabalho.
2. `git add <arquivo>` - Adiciona um arquivo específico à área de preparação (staging).
3. `git add .` - Adiciona todas as alterações do diretório de trabalho à área de preparação.
4. `git commit -m "mensagem do commit"` - Cria um novo commit com as alterações preparadas.
5. `git diff` - Mostra as diferenças entre o diretório de trabalho e a área de preparação.
6. `git log` - Exibe o histórico de commits.
7. `git log --oneline` - Exibe o histórico de commits em uma linha por commit.
8. `git log --graph` - Exibe o histórico de commits em forma de gráfico.

## Branches

1. `git branch` - Lista todos os branches locais e mostra o branch atual.
2. `git branch <nome_branch>` - Cria um novo branch com o nome especificado.
3. `git checkout <nome_branch>` - Muda para o branch especificado.
4. `git merge <nome_branch>` - Mescla o branch atual com o branch especificado.
5. `git branch -d <nome_branch>` - Deleta o branch especificado (deve estar mesclado).
6. `git branch -D <nome_branch>` - Deleta o branch especificado mesmo que não esteja mesclado.

## Atualização e Sincronização

1. `git fetch` - Busca as atualizações do repositório remoto (não mescla automaticamente).
2. `git pull` - Busca as atualizações e mescla automaticamente com o branch atual.
3. `git push <nome_remoto> <nome_branch>` - Envia os commits locais para o repositório remoto.

## Ignorar Arquivos

1. Criar um arquivo `.gitignore` e listar os arquivos/diretórios que devem ser ignorados.

## Desfazer Alterações

1. `git reset HEAD <arquivo>` - Remove um arquivo da área de preparação.
2. `git checkout -- <arquivo>` - Desfaz as alterações de um arquivo no diretório de trabalho.
3. `git revert <hash_do_commit>` - Cria um novo commit revertendo as alterações do commit especificado.

## Outros

1. `git remote add <nome_remoto> <URL>` - Adiciona um repositório remoto ao seu repositório local.
2. `git remote -v` - Lista os repositórios remotos configurados.
3. `git show <hash_do_commit>` - Mostra detalhes de um commit específico.
4. `git stash` - Salva as alterações atuais em uma pilha de mudanças temporárias (stash).
5. `git stash apply` - Aplica a última mudança da pilha de stash.
6. `git help` - Exibe a documentação de ajuda do Git.

