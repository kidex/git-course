# Git Workflow

## Pasi:

###  C1 - Daca avem nevoie de un branch nou de la inceput

1. **git status**
2. **git checkout `<nume-branch-principal>`** (de obicei e main sau master)
3. **git pull origin `<nume-branch-principal>`** (de obicei e main sau master)
4. **git checkout -b `<nume-branch-nou>`** (cream un branch nou, de preferat de forma "creez-un-branch-nou")
5. modificam codul (ceea ce mi se cere sa fac in task)
6. **git add -A** (adaugam modificarile - fisiere/foldere create/sterse, modificari de fisiere)
7. **git commit -m "mesaj"** (incarcam modificarile in commit)
8. **git push origin `<nume-branch-nou>`** (adaugam commit-ul in respository remote)
9. intram pe client (github.com/bitbucket.com/gitlab.com etc) si cream pull request
10. notificam reviewerii de noul pull request ridicat

###  C2 - Daca continuam munca pe un branch deja creat

1. **git status**
2. **git checkout `<nume-branch>`** (branch-ul pe care am lucrat)
3. **git pull origin `<nume-branch>`** (branch-ul pe care am lucrat)
4. modificam codul (ceea ce mi se cere sa fac in task)
5. **git add -A** (adaugam modificarile - fisiere/foldere create/sterse, modificari de fisiere)
6. **git commit -m "mesaj"** (incarcam modificarile in commit)
7. **git push origin `<nume-branch>`** (adaugam commit-ul in respository remote)
8. intram pe client (github.com/bitbucket.com/gitlab.com etc) si cream pull request 
9. notificam reviewerii de noul pull request ridicat

#### Nota de informare
In cazul in care, nu am terminat munca, nu respectam pasii de creare a Pull Request-ului (9, 10 in C1 si 8,9 in C2) 

#### Bune practici
1. Este bine sa dati commit chiar daca nu ati terminat task-ul dar ati incheiat ziua de munca
2. Mesajele de commit sa fie sugestive cu ce ati facut voi (ca si functionalitate nu modificari de fisiere)
3. Este bine ca in momentul in care dati commit sa nu aveti erori (comentati liniile/fisierele care dau erori mai bine)
4. In mod regulat sa tineti proiectul local la zi cu cel din remote (git pull origin main regulat)
