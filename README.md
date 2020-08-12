# Git e Github
- Como usar Git e Github na prática: Guia para iniciantes | Mayk Brito
- https://www.youtube.com/watch?v=2alg7MQ6_sI&t=259s

## Termos Git
- Git: é como uma árvore
- Master: é o caule dessa árvore
- Branch: Ramos
- Commits: são pontos na história

## Iniciando
- git config --global user.name "Seu nome"
- git config --global user.email "seu e-mail"
#

## Comandos Git

### `git init` // Iniciar um projeto com Git

### `git status` // Verificar status

### `git add` // Adicionar um ponto história
- git add nome-arquivo.extensão
- ou para add todos
git add .
- ou todos com uma determinada extensão
- git add -.html
- git add pasta/-.html
- git add pasta/-

### `git commit` // Criar um ponto na hostória
Commit com a mesagem para inidicar qual foi a alteração (agora tem um ponto na história)
- git commit -m 'Seu commit'
- (Exemplo de info):
- 1 arquivo com 12 linhas
- 1 file changed, 12 insertions(+)
- Nada para commitar
- nothing to commit, working tree clean

### `git commit -am "Seu commit"` // adiciona e já faz o commit

### `git log` // Ver as informações dos Commits que já foram feitos
- `git log -1` // mostrar apenas o ultimo commit
- `git log --oneline` // resumido em linhas
- `git log --oneline --all` // todos mesmo não estando no branch atual
- `git log --oneline --all --decorate` // mostar o que está em cada branch
- `git log --oneline --all --decorate --graph` // grafico
- para sair do git log tecla q

### `git show` // Ver o ultimo ponto
- `git show numeroDoCommit`
- Ex: git show af9301d7beeb1a5229e871fadf1aac41c6ad7f1f

### `git diff` // Verificar quais foram as alteraçõe nos arquivos - mostra o que foi realizado entes de dar um add

### `.gitignore` // Crie o arquivo .gitignore e coleque os diretorios e arquivos para serm ignorados

### `git checkout` // Ir para algum lugar 
- `git checkout` + numero do commit
- `git checkout` + nome da branch
- `git checkout master` // para voltar

### `cat` // Ver o conteudo de um arquivo no commit
- cat exemplo.html

### `git branch` // Ramos do projeto
- git branch nome-do-ramo
- Ex: git branch feature/nfe
- se der o camando git branch vai aparecer 2 branchs o master(caule) e feature/nfe(ramo)

### `git merge` // Merge: mesclar branch p/ master

### `git branch -D nome-da-branch`// Deletar uma branch

### `git remote` // Adicionar um repositorio remoto
- git remote add nome link-do-github
- Ex: git remote add origin https://github.com/rsaraceni/live-git.git

### `git remote -v` // Listar urls 

### `git push` // Enviar para o github remoto
- git push nome-do-ponto nome-do-ramo
- Ex: git push origin master

### `git clone` // Clonar projeto
- git clone url-do-projeto pasta
- Ex: git clone https://github.com/rsaraceni/live-git.git GitHub
- Caso já esteja na pasta do desejada é só:
- git clone https://github.com/rsaraceni/live-git.git

### `git pull` // puxar do github 
- git pull 
- git pull + remote a puxar + ramo
- Ex: git pull origin master

### `git config credential.helper store` // quando der um push não precisa das credencias
# 


## Ferramentas

### Travis
- Utilizando Travis CI como servidor de integração contínua em projetos open-source
https://travis-ci.org/
- https://medium.com/@mari_azevedo/utilizando-travis-ci-como-servidor-de-integra%C3%A7%C3%A3o-cont%C3%ADnua-em-projetos-open-source-um-exemplo-com-a-e30082f3ef46