## Staging and Commit (Preparação e Confirmação)
    a = add                           # Stage changes (Preparar alterações)
    aa = add -A                       # Stage all changes, including untracked files (Preparar todas as alterações, incluindo arquivos não rastreados)
    ap = add -p                       # Interactively stage changes (Preparar interativamente as alterações)

    c = commit --verbose              # Commit with verbose output (Confirmar com saída detalhada)
    ca = commit -a --verbose          # Commit all changes with verbose output (Confirmar todas as alterações com saída detalhada)
    cm = commit -m                    # Commit with a specified message (Confirmar com uma mensagem específica)
    cam = commit -a -m                # Commit all changes with a specified message (Confirmar todas as alterações com uma mensagem específica)
    m = commit --amend --verbose      # Amend the last commit with verbose output (Emendar o último commit com saída detalhada)

## Difference (Diferenças)
    d = diff                          # Show the difference between the working directory and last commit (Mostrar a diferença entre o diretório de trabalho e o último commit)
    ds = diff --stat                  # Show a summary of changes as a stat (Mostrar um resumo das alterações como estatísticas)
    dc = diff --cached                # Show the difference between the index (staged changes) and last commit (Mostrar a diferença entre o índice e o último commit)

## Status
    s = status -s                    # Show short status of changed files (Mostrar um status curto dos arquivos modificados)
    st = status                       # Show a detailed status (Mostrar um status detalhado)

## Checkout e Branch (Checkout and Branch)
    co = checkout                     # Checkout a branch or commit (Fazer checkout de um branch ou commit)
    cob = checkout -b                 # Create and checkout a new branch (Criar e fazer checkout de um novo branch)

## Desfazer o Stage (Unstage)
    unstage = restore --staged        # Unstage changes from the index (Desfazer o stage das alterações no índice)

## Listagem de Branches (Branch Listing)
    b = "!git for-each-ref --sort='-authordate' --format='%(authordate)%09%(objectname:short)%09%(refname)' refs/heads | sed -e 's-refs/heads/--'"  # List branches sorted by author date (Listar branches ordenados por data do autor)

## Listar Aliases (List Aliases)
    la = "!git config -l | grep alias | cut -c 7-"  # List Git aliases (Listar aliases do Git)

## Configuração (Configuration)
    config-name = config --global user.name "Seu Nome"                # Set global Git user name (Definir o nome de usuário Git global)
    config-email = config --global user.email "seu.email@example.com"  # Set global Git user email (Definir o email de usuário Git global)
    config-editor = config --global core.editor "editor"                # Set global Git text editor (Definir o editor de texto Git global)

## Inicialização de Repositório (Repository Initialization)
    init = init                        # Initialize a new Git repository (Inicializar um novo repositório Git)
    clone = clone                      # Clone a remote repository (Clonar um repositório remoto)

## Gerenciamento de Mudanças (Change Management)
    git-status = status                # Alias for 'status' (Alias para 'status')
    git-add = add                      # Alias for 'add' (Alias para 'add')
    git-commit = commit                # Alias for 'commit' (Alias para 'commit')
    git-diff = diff                    # Alias for 'diff' (Alias para 'diff')

## Branches 
    git-branch = branch                # Alias for 'branch' (Alias para 'branch')
    git-checkout = checkout            # Alias for 'checkout' (Alias para 'checkout')
    git-merge = merge                  # Alias for 'merge' (Alias para 'merge')

## Atualização e Sincronização (Update and Synchronize)
    git-fetch = fetch                  # Alias for 'fetch' (Alias para 'fetch')
    git-pull = pull                    # Alias for 'pull' (Alias para 'pull')
    git-push = push                    # Alias for 'push' (Alias para 'push')

## Ignorar Arquivos ( Ignore Files)
    git-ignore = "!echo 'arquivo_ou_diretório_a_ignorar' >> .gitignore"  # Ignore a file or directory in .gitignore (Ignorar um arquivo ou diretório no .gitignore)

## Desfazer Alterações (Undo Changes)
    git-reset = reset                  # Alias for 'reset' (Alias para 'reset')
    git-revert = revert                # Alias for 'revert' (Alias para 'revert')

## Outros (Others)
    git-remote-add = remote add        # Alias for 'remote add' (Alias para 'remote add')
    git-remote-list = remote -v        # Alias for 'remote -v' (Alias para 'remote -v')
    git-show = show                    # Alias for 'show' (Alias para 'show')
    git-stash = stash                  # Alias for 'stash' (Alias para 'stash')
    git-stash-apply = stash apply      # Alias for 'stash apply' (Alias para 'stash apply')
    git-help = help                    # Alias for 'help' (Alias para 'help')
