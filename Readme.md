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

//Criar arquivo .gitignore<br>
'[editor]' .gitignore.<br> Ex: code .gitignore

//Stash<br>
git stash<br>
git stash aplly<br>
git stash list<br>
git stash clear<br>

//Criando alias <br>
git config --global alias.<font color=green>s</font> status => git status => git s <br>

//Criando tags, releases<br>
git tag -a 1.0.0 -m "readme finzalizado"<br>
git push origin master --tags<br>
//Lista as tags: git tag<br>

git revert '[hash]'

//Excluir branch no repositório remoto
git tag -d 1.0.10 //Apaga localmente<br>
git push origin :'[branch ou tag]'<br>
git push origin :1.0.10 //Apaga remoto





