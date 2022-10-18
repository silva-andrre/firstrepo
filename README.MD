# Primeiro Repositório Git
## Introdução ao Git
Aprendendo comandos básicos do Git

Primeiros comando aprendidos:
	git init
	git status
	git add --all
	git commit -m "Mensagem"
	git log
	git log -p
	git checkout -- README.md

Novos comandos:
	git branch
	git checkout nomeBranch
	git checkout -b nomeBranch



Se quisermos desfazer as alterações em um arquivo antes de adicionar o mesmo na área de Stage para o próximo commit:

$ git checkout -- README.md
$ cat README.md
Se já tivermos adicionado as alterações na área de Stage:

$ git reset HEAD README.md
$ git checkout -- README.md
Se já tivermos feito o commit:

$ git reset --soft HEAD~1
$ git reset HEAD README.md
$ git checkout -- README.md
Esses foram rollbacks seguros, onde você sabe exatamente o que está desfazendo e por etapa. Existe uma opção mais agressiva caso você tenha certeza que quer desfazer todas as alterações do último commit:

$ git reset --hard HEAD~1
$ cat README.md
$ ls
$ git log
