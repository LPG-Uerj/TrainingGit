# TrainingGit

## Plano de Aula

Treinamento de GIT/GitHub

Instrutor: Jefson Rosa Florêncio

Disciplina: Estágio de Docência I

Professor: Guilherme Abelha

Primeira parte do treinamento (15 minutos): Apresentação de Slides sobre: O que é GIT? O que é GitHub? Para que serve? Como funciona?  Instalação; 

Segunda parte do treinamento: Exercícios Práticos (45 minutos):

## Exercício 1 – Configurando o GIT na máquina

	git config --global user.name “jefsonflorencio”
	git config --global user.email “jefsonflorencio@gmail.com”

## Exercício 2 – Criando uma conta no github.com

- sign up > e-mail > password > username > n > verifique a conta > Create account > valide com o código do e-mail > continue > continue for free.
- Criando um Personal Access Token
- Clique na foto > Settings > Developer settings > Personal access tokens > tokens (Classic) > Generate a personal access token

## Exercício 3 – Criando um repositório no github.com
- Create a new repository com o nome ‘treinamento_git’
- Copie o endereço do repositório criado e execute o comando abaixo no Terminal:
- git clone https://github.com/xxxxxxxxxx/treinamento_git.git



## Exercício 4 – Criando e gerenciando um projeto na máquina local

- Abra um Terminal e abra a pasta criada pelo git clone;
- Para tornar a pasta em um projeto/repositório GIT execute o comando:
	- git init
-  Para ver os status do projeto git:
	- git status
- Criando um arquivo README.md
	- echo "# treinamento_git" >> README.md
- Adicionando o arquivo README.md na stage commit:
	- git add README.md
- Versionando (Commitando)  o arquivo README.md:
	- git commit -m “create README.md”
- Verificando o log do GIT:
	- git log
- Altere o arquivo  README.md;
- Vendo a diferença entre as versões:
	- git diff
- Adicionando vários arquivos na stage commit:
	- git add .
- Retirando arquivos do stage commit:
	- git reset
- Revertendo um commit
	- git revert <hash_commit>
	- git log
	- git show <hash_commit>
- Subindo os arquivos para o repositório no GitHub:
	- git push -u origin main


## Exercício 5- Trabalhando com Branchs
- Criando um novo Branch:
	- git checkout -b nova_funcionalidade
- Crie um novo arquivo no novo branch
	- echo "# Hello World" >> index.txt
- Versionando o novo arquivo no novo branch
	- git add .
	- git commit -m “Create index.txt”
	- git push origin nova_funcionalidade
- Listando os Branchs
	- git branch -a
- Mudando de Branch
	- git checkout main
- Mesclando os branchs
	- git merge nova_funcionalidade
	- git push
- Apagando o novo branch
	- git branch -d nova_funcionalidade

## Exercício 6- Trabalhando com Forks
- acesse https://github.com/LPG-Uerj/TrainingGit
- Fork > Create a new fork > Create Fork
- Altere e commit o README.md
- Para alterar o projeto original do fork utilize a função “Pull Request” > new pull request > Create pull request 
- No projeto original vá em Pull Request para aceitar ou não as solicitações.
