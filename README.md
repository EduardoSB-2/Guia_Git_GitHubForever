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