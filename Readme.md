#GitHub

Primeiro arquivo do git

git status
git add <file>
git commit -m "mensagem"
git log --author "fulano"
git shortlog -sn

git diff
git diff --name-only

git reset HEAD<fileName> //Remover arquivo staged (após add)
git checkout <filename> //Desfazer alteração do arquivo antes do add
git reset --soft <hash> //Escolher hash anterior ao commit a serem feitas a reversão. Este comando deixa os arquivos em estado staged (pós add)
git reset --mixed <hash> //Mesma ação acima mas deixa os arquivos em estágio modified (pré add)
git reset --hard <hash> //Mata toda alteração daquela hash. Reversão mais bruto.

git remote add origin <url>
git remote -v