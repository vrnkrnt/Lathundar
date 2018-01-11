Git Lathund
===============

Bra länkar
-----------

[Tutorial med steg](http://try.github.io/)

Hjälp
-----------

Help:
`git help`

Standard
-----------

Initiera Git:
`git init`

Adda alla filerna för att sen commita:
`git add -A`

Adda speciel fil för att sen commita:
`git add index.html`

Committa ändringar:
`git commit -m "Meddelande"`

Add och commit i ett steg:
`git commit -am "Meddelande"`

Radera filer från Git:
`git rm index.html`

Uppdatera och radera
-----------

Lägg till fil och/eller ändra senaste commit meddelandet:
`git commit --amend -m "Meddelande"`

Uppdatera senaste commit meddelandet:
`git commit --amend -m "Nytt Meddelande"`

Branch
-----------

Visa brancherna (+ `-a` för att se alla):
`git branch`

Skapa branch:
`git branch branchNamn`

Ändra branch:
`git checkout branchNamn`

Skapa och ändra till ny branch:
`git checkout -b branchNamn`

Döpa om branch:
`git branch -m branchNamn new_branchNamn` or:
`git branch --move branchNamn new_branchNamn`

Radera merged/samanfogad branch (bara möjligt om det inte är HEAD):
`git branch -d branchNamn` eller:
`git branch --delete branchNamn`

Merge
-----------

Samanfoga brancher (upstram):
`git merge branchNamn`


Gitignore & Gitkeep
-----------

Skapa en tom textfil med .gitignore för att få med mappen dör filen ligger

Add eller ändra gitignore: 
`nano .gitignore`

Hitta tomma mappar: 
`touch dir/.gitkeep`

Log
-----------

Visa commits:
`git log`


Sammarbeta
-----------

Visa remote:
`git remote`

Visa remote detaljer:
`git remote -v`

Lägg till remote origin från GitHub projekt:
`git remote add origin https://github.com/user/project.git`

Visa alla branches:
`git branch -a`

Jämföra skillnaderna i brancher:
`git diff origin/master..master`

Push (ställ in standard `-u`):
`git push -u origin master`

Push till standard:
`git push origin master`

Pull:
`git pull`

Pull specifik branch:
`git pull origin branchNamn`

Merge hämtade commits:
`git merge origin/master`

Clona till localhost:
`git clone https://github.com/user/project.git`

Randera remote branch (pusha ingenting):
`git push origin :branchNamn` eller:
`git push origin --delete branchNamn`

Allmänt
-----------

### Steg för att ladda upp en mapp till GitHub 

1. Gå in i mappen (`git bash` i mappen eller `cb 'mappen'` i cmd)
2. `git init`
3. `git status`
4. `git add 'fil'` (eller `git add -A` om man vill adda alla filer i mappen)
5. `git commit -m "Meddelande om ändringar eller vad man gjort med filen"`. Add rep på GitHub, följ instruktionerna (alt. 2: `git remote add origin https://....` , `git push -u origin branchname`)
6. För att pusha igen, gör steg 3-5 och skriv sen `git push`

### Fork  
>Om man klickar på 'Fork' i någon annas rep skapas en kopia på samma rep men i ens egna profil där du kan ändra/kommentera och sen submitta en pull request till ägaren för att h*n ska kunna se ändringarna. Man kan också se om någon annan har ändrat/kommenterat sina filer under fliken 'Pull requests' i reppet. 
>
>[Hur `fork` funkar](https://help.github.com/articles/fork-a-repo/)

### Clone 
>Gå till ett rep, klicka på 'clone/download', kopiera URLen för reppet Öppna git bach i mappen du vill att den ska ligga i. Skriv git clone och URLen, tryck enter
>
>[Hur `cloning` finkar](https://help.github.com/articles/cloning-a-repository/)

### Push   
>För att ladda up arbetet till GitHub måste man pusha det. 
>	
>1. `git remote add origin https://....`
>2. `git push -u origin branchname`

### Add 
>För att lägga till filerna i Git så att man kan nå dom från olika datorer och inte bara ha dom lokalt

### Commit
>För att lägga till ett meddelande i filerna som man pushar till GitHub. Bra om man är noggrann och konsekvent med det man lägger till som meddelande.