Git Lathund
===============

Bra länkar
-----------

Tutorial: http://try.github.io/


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
