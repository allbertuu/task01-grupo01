# task01-grupo01
💙🚀 Primeira task do Vem Ser DBC 11ª edição, realizada pelo Grupo 01 (Claudio Henrique, Alberto Albuquerque e o Gustavo Assis)

# Rebase
Move ou combina uma sequência de commits para uma novo commit base.
## Sintaxe
```shell
git rebase <base>
```
## Uso
```shell
git rebase main
```

# Cherry pick
Aplica as mudanças de outros commits existentes, gerando um novo commit pra cada.
## Sintaxe
```shell
git cherry-pick [--edit] [-n] [-m <parent-number>] [-s] [-x] [--ff]
          [-S[<keyid>]] <commit>…​
git cherry-pick (--continue | --skip | --abort | --quit)
```
## Uso
```shell
git cherry-pick f13bd3c3531f26e805c606729857f39987a2420f
```

# Revert
Reverte alguns commits existentes. Esse comando faz é basicamente desfazer tudo aquilo que foi feito dentro de um determinado commit
## Sintaxe
```shell
git revert [--[no-]edit] [-n] [-m parent-number] [-s] [-S[<keyid>]] 
  <commit>…​
git revert (--continue | --skip | --abort | --quit) 
```
## Uso
```shell
git revert HEAD
```

 # Squash
Agrupa mais de um commit em um commit selecionado.
## Sintaxe
```shell
git rebase -i [hashcode]
```
## Uso
Esse comando mostra uma lista de commits, dessa forma:
    
    pick fb554f5 commit 1
    s 2bd1903 commit 2
    s d987ebf commit 3

    # Rebase 9cbc329..d987ebf onto 9cbc329
    #
    # Commands:
    # p, pick = use commit
    # r, reword = use commit, but edit the commit message
    # e, edit = use commit, but stop for amending
    # s, squash = use commit, but meld into previous commit
    # f, fixup = like "squash", but discard this commit's log message
    # x, exec = run command (the rest of the line) using shell
    #
    # If you remove a line here THAT COMMIT WILL BE LOST.
    # However, if you remove everything, the rebase will be aborted.
