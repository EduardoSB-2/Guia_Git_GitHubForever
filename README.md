# Guia definitivo sobre Git e GitHub

## Iniciando um Repositório

- Instalar o Git no Computador ( Sendo ele um software de versionamento local)

- 2° Passo: Configurar o software de Versionamento

- git config --global user.name "Username"
- git config --global user.email "meu@email.com"
- Verificação do git: git --version
- Verificação da maquina configurada: git config --list

3° Passo: Iniciar o Repositorio Local

- git init (Cria o ambiente de versionamento na pasta do projeto)

4° Passo: Iniciar o Repositorio Online (GitHub) e Linkar o meu repositorio remoto ao local -- GIT <-> GITHUB

- git remote add origin + link do repositorio do Github
- git remote get-url origin (verifica o link)
- git remote set-url origin + link do repositorio do Github (modifica o link)

5° Passo: Adicionar meus Arquivos ao Repositório Local
- git add + nome do arquivo
- git add . (Adiciona todos os arquivos de uma única vez)

6° Passo: Git Commit - Criar o Versionamento Local
- git commit -m "Sua Mensagem"

7° Passo: Sincronização do Repositorio Local com o  Online (GITHUB)
- git push -u origin main

8° Passo: Clonar um Repositorio da Nuvem
- git clone + link do repositório do Github

9° Passo: Atualizar um Repositorio Local
- git pull origin main

///////////////////////////////////////////////////////////

## Criando um Repositório Colaborativo

### Para usarem um projeto:
- Clone o projeto git clone https://github.com/seu-projeto.git
- Para contribuir com esse projeto, entre na sua branch(seu nome) git checkout <nome_branch> e digite git pull origin main para trazer os dados mais recentes da main.

- Ao terminar sua contribuição, faça push para o servidor remoto no branch que você criou. Por exemplo:
- git add .
- git commit -m "mensagem do commit"
- git push -u origin <nome_branch>

- Crie um novo PULL REQUEST no repositório, para que o seu branch seja analisado e, se estiver correto, seja adicionado ao branch main pelo gerente do projeto.

- Atualizando sua Branch com a Última Versão da main, assim antes de começar a trabalhar em uma nova tarefa ou após terminar de trabalhar em sua branch, é importante garantir que sua cópia local da branch main esteja sempre atualizada. Para isso, siga os passos abaixo para puxar as últimas atualizações de main:

1. Vá para a Branch main
Primeiro, certifique-se de que você está na branch main, onde todas as atualizações principais do projeto estão sendo feitas.

- git checkout main git pull origin main

Voltando para sua Branch de Trabalho e Fazendo o Merge com main.
Após garantir que a branch main está atualizada, o próximo passo é voltar para a sua branch de trabalho e integrar as últimas alterações da main nela. Isso garante que você esteja trabalhando com a versão mais atualizada do projeto, evitando conflitos futuros ao fazer o merge de volta para a develop. Siga os passos abaixo:

1. Volte para a Sua Branch de Trabalho
Se você estava na branch main para atualizar o código, agora é hora de voltar para a sua branch de trabalho, onde você estava desenvolvendo suas alterações. Use o seguinte comando para mudar para a sua branch de trabalho:

- git checkout <nome_da_sua_branch>

- git merge main
