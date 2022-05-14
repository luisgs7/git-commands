# Principais comandos do GIT

Git Log

```
git shortlog
```

```
git log --decorate
```

```
git shortlog -sn
```

```
git log --graph
```
<br>
Git Diff

```
git diff
```

```
git diff --name-only
```

Git Commit

```
git commit -am "New commit"
```

```
git show <id-commit>
```

Voltar o estado do arquivo para antes de uma edição

```
git checkout <file-name>
```

Voltar o estado para antes de ter executado o comando ``` git add <file-name> ```

```
git checkout HEAD <file-name>
```

Git reset

#### Mais Indicado
```
git reset --soft <id-commit-anterior>
```

```
git reset --mixed <id-commit-anterior>
```
Não utilizar!!! 
```
git reset --hard <id-commit-anterior>
```

Git Branch

Criar uma nova branch
```
git checkout -b <name-new-branch>
```

Listar as branchs
```
git branch
```

Mudar de branchs
```
git checkout <name-branch>
```

Deletar uma branch
```
git branch -D <name-branch>
```

Git Merge (Utilizar em caso de pull request)

```
git merge <branch-name>
```

Git Rebase

```
git rebase <branch-name>
```

Git Stash

Salva uma modificação para ser alterada depois
```
git stash
```


```
git stash list
```

```
git stash apply
```

Git Alias

##### Criando um alias para o comando status
```
git config --global alias.s status
```

```
git s
```

Git Tag

```
git tag -a 1.0.0 -m "README FILE"
```

```
git push origin main --tags
```

```
git tag
```

Git Revert

Comando muito importante, pois a partir dele é possível reverter o último commit,
entretanto o último commit não é apagado, como no merge ou rebase, apenas é 
criado um novo commit com o snapshot do commit anterior

```
git revert <id-commit-com-bug>
```