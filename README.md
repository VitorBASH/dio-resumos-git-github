
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
| Salvando alterações no repositório local | [Video]() | 

## Comandos - Configurando o git

- **```git config --global user.name "[nome de usuário]"```** - Define o nome de usuário em todos os repositórios.
- **```git config --global user.email "[e-mail]"```** - Define um endereço de email em todos os repositórios.
- **```git config user.[name ou email]```** - Mostra o nome ou email do usuário dos repositórios.

- **```git config init.defaultBranch```** - Mostra o nome da Branch padrão.

- **```git config --global init.defaultBranch main```** - Define o nome da sua Branch padrão em todos os repositórios.

## Comandos - Autenticando via Token

- **```git clone [URL do repositório]```** - Clona um repositório do GitHub

- **```git config --global credential.helper [store ou cache]```** - Salva a credencial no PC; STORE: permanente | CACHE: temporário.
- **```git config --global credential.helper```** - Verifica o tipo de credencial salva.