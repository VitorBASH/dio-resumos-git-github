
# DIO | Resumos Git e GitHub

Repositórios para armazenar resumos sobre Git e GitHub do curso Versionamento de Código com Git e GitHub.

## Documentação
- [Ducomentação Git](https://git-scm.com/doc)
- [Documentação GitHub](https://docs.github.com/pt)

## Resumos das Aulas

| Aulas | Resumos |
|------|---------|
| Configurando o Git| [Video](https://web.dio.me/course/versionamento-de-codigo-com-git-e-github/learning/f9b294d2-f8ca-4364-9031-1e897721b3e2?autoplay=1&back=%2Ftrack%2Fsantander-linux-para-iniciantes&moduleId=undefined&tab=undefined) |
| Autenticando via Token | [Video](https://web.dio.me/course/versionamento-de-codigo-com-git-e-github/learning/3d13d85f-2508-4396-9657-4643d3302c79?autoplay=1&back=%2Ftrack%2Fsantander-linux-para-iniciantes&moduleId=undefined&tab=undefined) |
| Criando e Clonando repositórios | [Video](https://web.dio.me/course/versionamento-de-codigo-com-git-e-github/learning/a377a00b-461c-4ab0-8258-3addd2fef14c?autoplay=1&back=%2Ftrack%2Fsantander-linux-para-iniciantes&moduleId=undefined&tab=undefined)
| Salvando alterações no repositório local | [Video](https://web.dio.me/course/406684a4-396d-4160-94b9-ead934e18564/learning/599dd3dd-d189-474f-a55c-22f37b4472da?autoplay=1&back=%2Ftrack%2Fsantander-linux-para-iniciantes&moduleId=undefined&tab=undefined) | 

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