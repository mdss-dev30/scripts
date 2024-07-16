### configurando user:

git config --global user.name "SEU NOME"

git config --global user.email seuemail@example.com

### criar chave ssh:

ssh-keygen -t ed25519 -C "seuEmail@seuEmail.com.br"

### iniciar agent ssh:

eval $(ssh-agent -s)

### informar para o agent sua chave priv:

ssh-add "o caminho da sua chave ex: /home/seuUsuario/.ssh/id_numeroDaChavePrivada"

### mostrar quais repositórios remotos estão associados:

git remote -v

### iniciar um repositorio

git init

### exibir informções do repositorio

git status

### adicionar arquivos todos os arquivos 
git add .

### adicionar mensagem descrevendo o commit

git commit -m "mensagem do commit"

### git log

https://devhints.io/git-log

### ver qual branch vc esta trabalhando

git branch

### criar uma nova branch

git branch nome-da-branch

### mudar de branch

git checkout nome-da-branch

### unir duas branchs

git merge nome-da-branch(que irá unir com a atual)

### colocando os commits na ordem de criação e fazendo merge

git rebase nome-da-branch(que irá unir com a atual)

##O merge junta os trabalhos e gera um merge commit. O rebase aplica os commits de outra branch na branch atual.

### Com o git checkout nós desfazemos uma alteração que ainda não foi adicionada ao index ou stage, ou seja, antes do git add. Depois de adicionar com git add, para desfazer uma alteração, precisamos tirá-la deste estado, com git reset. Agora, se já realizamos o commit, o comando git revert pode nos salvar.

### pausar o desenvolvimento atual para continuar depois

git stash

### ver area do stash

git stash list

### continuar o desenvolvimento 

git stash apply 0(numero do stash)

### apagar area do stash

git stash drop

### pegar a última alteração adicionada à stash, e já removê-la de lá

git stash pop

### verificar o que foi alterado

git diff ea539b3 (até) .. 6ca12ac

### criar uma tag no seu código

git tag -a v0.1.0(nome ou versão da tag)

### enviar esta tag para o GitHub

git push v0.1.0(nome ou versão da tag)

### ver tags 

git tag