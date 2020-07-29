#GitHub

Primeiro arquivo do git

git status
<br>
git add '[file]'
<br>
git commit -m "mensagem"
<br>
git log --author "fulano"
<br>
git shortlog -sn
<br>

git diff
<br>
git diff --name-only
<br>

git reset HEAD '[fileName]' //Remover arquivo staged (após add)
<br>
git checkout '[filename]' //Desfazer alteração do arquivo antes do add
<br>

git reset --soft '[hash]' //Escolher hash anterior ao commit a serem feitas a reversão. Este comando deixa os arquivos em estado staged (pós add)
<br>

git reset --mixed '[hash]' //Mesma ação acima mas deixa os arquivos em estágio modified (pré add)<br>
git reset --hard '[hash]' //Mata toda alteração daquela hash. Reversão mais bruto.
<br>

git remote add origin '[url]'<br>
git remote -v

//Criar branch
git checkout -b '[nomeBranch]'

//Excluir um branch
git checkout -D '[nomeBranch]'

//Merge
//na master: git merge '[branch]'

//Rebase
na master: git rebase '[branch]'

//Criar arquivo .gitignore
[editor] .gitignore.<br> Ex: code .gitignore

//Stash<br>
git stash<br>
git stash aplly<br>
git stash list<br>
git stash clear<br>