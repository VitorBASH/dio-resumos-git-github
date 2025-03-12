
# DIO | Resumos Git e GitHub

Repositórios para armazenar resumos sobre Git e GitHub do curso Versionamento de Código com Git e GitHub.

## Documentação
- [Ducomentação Git](https://git-scm.com/doc)
- [Documentação GitHub](https://docs.github.com/pt)

## Resumos das Aulas

| Aulas | Conteúdos |
|------|----|
| Configurando o Git| [Video](https://web.dio.me/course/versionamento-de-codigo-com-git-e-github/learning/f9b294d2-f8ca-4364-9031-1e897721b3e2?autoplay=1&back=%2Ftrack%2Fsantander-linux-para-iniciantes&moduleId=undefined&tab=undefined) / [Comandos](https://github.com/VitorBASH/dio-resumos-git-github?tab=readme-ov-file#comandos---configurando-o-git) |
| Autenticando via Token | [Video](https://web.dio.me/course/versionamento-de-codigo-com-git-e-github/learning/3d13d85f-2508-4396-9657-4643d3302c79?autoplay=1&back=%2Ftrack%2Fsantander-linux-para-iniciantes&moduleId=undefined&tab=undefined) / [Comandos](https://github.com/VitorBASH/dio-resumos-git-github?tab=readme-ov-file#comandos---autenticando-via-token)|
| Criando e Clonando repositórios | [Video](https://web.dio.me/course/versionamento-de-codigo-com-git-e-github/learning/a377a00b-461c-4ab0-8258-3addd2fef14c?autoplay=1&back=%2Ftrack%2Fsantander-linux-para-iniciantes&moduleId=undefined&tab=undefined) / [Comandos](https://github.com/VitorBASH/dio-resumos-git-github?tab=readme-ov-file#comandos---criando-e-clonando-reposit%C3%B3rios)|
| Salvando alterações no repositório local | [Video](https://web.dio.me/course/406684a4-396d-4160-94b9-ead934e18564/learning/599dd3dd-d189-474f-a55c-22f37b4472da?autoplay=1&back=%2Ftrack%2Fsantander-linux-para-iniciantes&moduleId=undefined&tab=undefined) / [Comandos](https://github.com/VitorBASH/dio-resumos-git-github?tab=readme-ov-file#comandos---salvando-altera%C3%A7%C3%B5es-no-reposit%C3%B3rio-local)|
| Desfazendo alterações no repositório local| [Video](https://web.dio.me/course/versionamento-de-codigo-com-git-e-github/learning/3f9f2336-6fd5-44cb-ba39-d1a4f6448023?autoplay=1&back=%2Ftrack%2Fsantander-linux-para-iniciantes&moduleId=undefined&tab=undefined) / [Comandos](https://github.com/VitorBASH/dio-resumos-git-github?tab=readme-ov-file#comandos---desfazendo-altera%C3%A7%C3%B5es-no-reposit%C3%B3rio-local)|
| Enviando e Baixando alterações em repositórios| [Video](https://web.dio.me/course/versionamento-de-codigo-com-git-e-github/learning/dd17c56e-2327-493c-942a-358a49a26549?autoplay=1&back=%2Ftrack%2Fsantander-linux-para-iniciantes&moduleId=undefined&tab=undefined) / [Comandos](https://github.com/VitorBASH/dio-resumos-git-github?tab=readme-ov-file#comandos---enviando-e-baixando-altera%C3%A7%C3%B5es-em-reposit%C3%B3rios)|
| Trabalhando com Branches 1 | [Video](https://web.dio.me/course/versionamento-de-codigo-com-git-e-github/learning/2c7fd2b1-e7c4-4947-9b07-ffcbfb4bd689?autoplay=1&back=%2Ftrack%2Fsantander-linux-para-iniciantes&moduleId=undefined&tab=undefined) / [Comandos](https://github.com/VitorBASH/dio-resumos-git-github?tab=readme-ov-file#comandos---trabalhando-com-branches-1)|
| Trabalhando com Branches 2 | [Video](https://web.dio.me/course/versionamento-de-codigo-com-git-e-github/learning/80018fab-daac-4917-8527-a6be2e0c3cf0?autoplay=1&back=%2Ftrack%2Fsantander-linux-para-iniciantes&moduleId=undefined&tab=undefined) / [Comandos](https://github.com/VitorBASH/dio-resumos-git-github?tab=readme-ov-file#comandos---trabalhando-com-branches-2)|

### Comandos - Configurando o git

- **```git config --global user.name "[nome de usuário]"```** - Define o nome de usuário em todos os repositórios.
- **```git config --global user.email "[e-mail]"```** - Define um endereço de email em todos os repositórios.
- **```git config user.[name ou email]```** - Mostra o nome ou email do usuário dos repositórios.
- **```git config init.defaultBranch```** - Mostra o nome da Branch padrão.
- **```git config --global init.defaultBranch main```** - Define o nome da sua Branch padrão em todos os repositórios.


### Comandos - Autenticando via Token


- **```git config --global credential.helper [store ou cache]```** - Salva a credencial no PC; STORE: permanente | CACHE: temporário.
- **```git config --global credential.helper```** - Verifica o tipo de credencial salva.


### Comandos - Autenticando via SSH

- **```ls -al ~/.ssh```** - Lista arquivos de SSH se existirem.
- **```ssh-keygen -t ed25519 -C [seu email]```** - Gera uma chave SSH.
- **```eval "$(ssh-agent -s)"```** - Inicia o ssh-agent.
- **```ssh-add ~/.ssh/id_ed25519```** - Adiciona sua chave SSH privada ao ssh-agent.


### Comandos - Criando e Clonando repositórios


- **```git init```** - Inicia um repositório Git.
- **```git clone [URL do repositório] [novo nome]```** - Clona um repositório do GitHub e pode ser renomeado.
- **```git clone [URL do repositório] --branch [nome da branch] --single-branch```** - Clona a branch especifica.
- **```git remote add origin [URL do repositório]```** - Vincula o repositório local com o remoto.


### Comandos - Salvando alterações no repositório local


- **```git status```** - Mostra o status de alterações.
- **```git add```** - Adiciona arquivos e diretórios à area de preparação.
- **```git commit -m"[comentário]"```** - Grava as alterações feitas no repositório local e cria um ponto de controle comentado.
- **```git log```** - Exibe o histórico de commits do repositório.
- **```echo [diretório ou arquivo]/ > .gitignore```** - Informa o Git para ignorar estes diretórios ou arquivos.


### Comandos - Desfazendo alterações no repositório local


- **```rm -rf .git```** - Deixa de ser um repositório Git.
- **```git restore [nome do arquivo ou diretório]```** - Restaura as alterações feitas desde o ultimo commit.
- **```git commit --amend -m"[novo comentário]"```** - Muda o comentário do ultimo commit.
- **```git reset --[soft, mixed, hard] [ID do commit]```** - Restaura para o commit selecionado. **Cuidado com o HARD!!!**
- **```git reflog```** - Mostra todo o histórico de commits (mesmo os deletados).
- **```git reset [arquivo ou diretório]```** - Retirar arquivos e diretórios da area de preparação.


### Comandos - Enviando e Baixando alterações em repositórios


- **```git remote add origin [URL do repositório]```** - Conecta o repositório local com o remoto.
- **```git push -u origin main```** - Envia o conteúdo do repositório local para o remoto.
- **```git pull```** - Baixa as alterações do repositório remoto para o local.


### Comandos - Trabalhando com Branches 1


- **```git checkout -b [nome da branch]```** - Cria e troca a Branch.
- **```git checkout [nome da branch] ```** - Troca a Branch.
- **```git branch -v```** - Mostra o ultimo commit de cada Branch.
- **```git merge [nome da branch]```** - Mescla as alterações das Branch.
- **```git branch```** - Mostra as Branch existentes.
- **```git branch -d [nome da branch]```** - Deleta a Branch.


### Comandos - Trabalhando com Branches 2


- **```git fatch origin main```** - Baixa as alterações do repositório remoto para branch main.
- **```git diff [branch] origin/[branch]```** - Verifica a diferença entre a Branch local e remota.
- **```git merge origin/main```** - Baixa a alterações da branch remota para a local.
- **```git clone [URL do repositório] --branch [nome da branch] --single-branch```** - Clona a branch especifica do repositório.
- **```git stash```** - Salva as alterações temporariamente e retorna para o ultimo commit.
- **```git stash list```** - Listar todos os stashes.
- **```git stash apply [ou nome do stash]```** - Aplica o stash mais recente ou o selecionado.
- **```git stash drop [nome do stash]```** - Remove o stash da lista após o uso.
- **```git stash pop```** - aplica o stash mais recente e remove automaticamente da lista.