# TOTUL DESPRE GIT


## Capitolul 1: Introducere în Git și Sistemele de Control al Versiunilor

### Capitolul 1: Introducere în Git

### 1.1 Ce este Git?
- Definiție și scop
- Istoricul și dezvoltarea Git

### 1.2 Instalarea Git
- Instalarea pe Windows
- Instalarea pe macOS
- Instalarea pe Linux

### 1.3 Configurarea Git
- Configurarea numelui și a e-mailului
- Alte setări de bază

## Capitolul 2: Concepte de Bază în Git

### 2.1 Repositories
- Definiție și scop
- Tipuri de repository-uri (local și remote)
- Inițializarea unui repository local

### 2.2 Staging și Commiting
- Stările fișierelor (untracked, staged, modified)
- Procesul de adăugare și commit
    - Comanda `git add`
    - Comanda `git commit`
- Comentarii în cod pentru fiecare pas al procesului

### 2.3 Vizualizarea Istoricului
- Comanda `git log`
- Interpretarea rezultatelor și utilizarea istoricului

## Capitolul 3: Ramificări și Măsurarea Conflictului

### 3.1 Ramificări (Branches)
- Definiție și utilizare
- Crearea unei ramuri noi
    - Comanda `git checkout -b`
- Combinarea ramurilor (merging)
    - Comanda `git merge`
- Rezolvarea conflictelor
    - Procesul și comenzi pentru rezolvarea conflictelor

### 3.2 Recomandări pentru Utilizarea Ramurilor
- Folosirea ramurilor pentru funcționalități noi și corectarea erorilor
- Menținerea ramurilor actualizate

## Capitolul 4: Lucrul cu Repositories Remote

### 4.1 Configurarea unui Remote Repository
- Adăugarea unui remote repository
    - Comanda `git remote add`

### 4.2 Împingerea și Tragerea Modificărilor
- Împingerea modificărilor
    - Comanda `git push`
- Tragerea modificărilor
    - Comanda `git pull`

### 4.3 Clonarea unui Repository
- Comanda `git clone`
- Utilizarea repository-ului clonat

## Capitolul 5: Tranzacții Avansate cu Git

### 5.1 Revertirea Modificărilor
- Utilizarea comenzii `git revert`
- Exemple de revertire a modificărilor

### 5.2 Resetarea Modificărilor
- Utilizarea comenzii `git reset`
- Diferența între resetare soft și hard

### 5.3 Stash
- Utilizarea comenzii `git stash`
- Aplicarea și gestionarea stash-urilor

## Capitolul 6: Practici Recomandate

### 6.1 Mesaje de Commit
- Scrierea mesajelor de commit clare și descriptive

### 6.2 Fă Commit-uri Frecvente
- Importanța commit-urilor frecvente

### 6.3 Revizuirea Codului
- Utilizarea pull requests (PR) pentru revizuirea codului
- Importanța revizuirii codului pentru menținerea calității

## Capitolul 7: Resurse Suplimentare

### 7.1 Documentație Oficială
- Link-uri și resurse pentru documentația oficială Git

### 7.2 Tutoriale și Cursuri
- Link-uri către tutoriale și cursuri online

### 7.3 Comunități și Forumuri
- Link-uri către comunități și forumuri de suport

## Anexe
- Ghid rapid de comenzi Git esențiale.
- Exemple de `.gitignore` pentru diverse tipuri de proiecte.
- Exemple de workflow-uri Git într-un mediu colaborativ.

# **Curs Git: Ghid Practic pentru Începători**

## Capitolul 1: Introducere în Git

### 1.1 Ce este Git?

Git este un sistem de control al versiunilor distribuit, utilizat pentru a urmări modificările aduse fișierelor într-un proiect. Permite colaborarea eficientă între mai mulți dezvoltatori, oferind funcționalități avansate pentru gestionarea istoricelor de modificări și a ramificărilor codului.

Git a fost creat de Linus Torvalds în 2005 pentru a sprijini dezvoltarea kernelului Linux. De-a lungul timpului, Git a devenit un instrument esențial în dezvoltarea software-ului, folosit de echipe de toate dimensiunile pentru a gestiona codul sursă și a coordona activitățile dezvoltatorilor.

### 1.2 Instalarea Git

Pentru a începe să folosești Git, trebuie să îl instalezi pe sistemul tău. Pașii pentru instalare variază în funcție de sistemul de operare.

#### Pe Windows:
1. Descarcă Git de la [site-ul oficial](https://git-scm.com/downloads).
2. Rulați installerul și urmați instrucțiunile pentru a finaliza instalarea.

#### Pe macOS:
1. Deschideți Terminalul.
2. Folosiți Homebrew pentru a instala Git: `brew install git`.

#### Pe Linux:
1. Deschideți terminalul.
2. Utilizați managerul de pachete al distribuției dvs. pentru a instala Git. De exemplu, pe Ubuntu: `sudo apt-get install git`.

### 1.3 Configurarea Git

După instalare, este important să configurezi Git cu informațiile tale de utilizator. Aceste setări vor fi incluse în commit-urile tale pentru a le asocia cu numele și adresa ta de e-mail.

```bash
# Configurare nume și e-mail
git config --global user.name "Numele Tău"
git config --global user.email "emailul@tau.com"
```

Aceste comenzi setează informațiile de bază care vor fi incluse în fiecare commit pe care îl faci.

---

## Capitolul 2: Concepte de Bază în Git

### 2.1 Repositories

Un repository (sau repo) este locul unde Git stochează toate fișierele și istoricul de modificări ale unui proiect. Există două tipuri principale de repository-uri:

- **Local Repository**: Se află pe computerul tău local.
- **Remote Repository**: Este găzduit pe un server la distanță, de obicei pe platforme precum GitHub, GitLab sau Bitbucket.

Pentru a iniția un repository local, folosești comanda:

```bash
git init
```

Această comandă creează un nou repository Git în directorul curent.

---

### 2.2 Staging și Commiting

Fișierele tale pot trece prin mai multe stări în Git. Imaginează-ți că lucrezi la un proiect de dezvoltare a unui site web. Tocmai ce ai creat o nouă pagină HTML pentru secțiunea de "Contact" și vrei să adaugi modificările în Git. În acel moment, fișierul este în starea de **untracked**, ceea ce înseamnă că Git încă nu îl urmărește.

După ce decizi să-l adaugi în Git folosind comanda `git add`, fișierul intră în starea de **staged**, adică este pregătit pentru a fi confirmat într-un commit. Ulterior, dacă faci modificări pe acest fișier, el va intra în starea de **modified**, indicând că există schimbări care nu au fost încă salvate într-un commit. Acest ciclu al stărilor fișierelor te ajută să urmărești fiecare etapă a dezvoltării.

Să presupunem că tocmai ai creat un fișier `contact.html` pentru secțiunea de "Contact" a unui site. Procesul ar putea arăta astfel:

```bash
# Creăm noul fișier HTML pentru pagina de contact
touch contact.html

# Verificăm starea fișierelor în Git. "contact.html" apare ca untracked.
git status
# Output:
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#         contact.html

# Adăugăm fișierul în zona de staging, pregătindu-l pentru un commit
git add contact.html

# Verificăm din nou starea. Acum fișierul "contact.html" este în staging.
git status
# Output:
# Changes to be committed:
#   (use "git restore --staged <file>..." to unstage)
#         new file:   contact.html

# Facem un commit cu un mesaj care explică adăugarea noii pagini
git commit -m "Adaugă pagina de contact"
# Output:
# [master 123abc] Adaugă pagina de contact
#  1 file changed, 0 insertions(+), 0 deletions(+)
#  create mode 100644 contact.html
```

#### Pasi de urmat

```bash
# Pasul 1: "touch contact.html" creează un fișier gol numit contact.html.
# La acest punct, fișierul este în starea de "untracked", ceea ce înseamnă că Git încă nu îl monitorizează.
# Pasul 2: "git status" ne arată că fișierul contact.html este untracked.
# Pasul 3: "git add contact.html" adaugă fișierul în zona de staging, unde Git îl pregătește pentru un commit.
# Pasul 4: "git status" arată că fișierul este acum în starea "staged", gata să fie confirmat.
# Pasul 5: "git commit -m 'Adaugă pagina de contact'" creează un commit, care salvează modificările făcute.
```

Acest proces este utilizat zilnic de dezvoltatori care lucrează la proiecte mari sau mici. Fiecare fișier nou creat într-un proiect trebuie să fie adăugat în Git pentru a fi urmărit. De exemplu, atunci când lucrezi la un site și creezi o nouă pagină sau un fișier CSS, acest fișier va trece prin etapele **untracked**, **staged**, și eventual **committed**. În acest fel, poți păstra un istoric detaliat al fiecărei modificări și poți colabora eficient cu echipa ta.

---

### 2.3 Vizualizarea Istoricului

Git păstrează un istoric detaliat al tuturor commit-urilor efectuate. Comanda `git log` este folosită pentru a vizualiza acest istoric, oferind informații despre fiecare commit, inclusiv mesajul acestuia, autorul și data.

```bash
git log
# Output (exemplu):
# commit 94f1e28393a4bc6a45d4a2a9d81e87f857b3b3f4 (HEAD -> master)
# Author: Nume Utilizator <emailul@tau.com>
# Date:   Fri Sep 6 12:34:56 2023 +0300
#
#     Adaugă pagina principală index.html
```

#### Pasi de urmat

```bash
# Pasul 1: "git log" afișează commit-urile recente, împreună cu autorul, data și mesajul descriptiv.
# Pasul 2: Fiecare commit conține un hash unic, care este identificatorul acelui commit.
# Pasul 3: Autorul commit-ului și data oferă informații despre cine și când a făcut schimbările.
# Pasul 4: Mesajul commit-ului explică clar ce a fost schimbat sau adăugat în cadrul acelui commit.
```

Această practică este extrem de utilă atunci când lucrezi într-o echipă de dezvoltare. Istoricul commit-urilor oferă o cronologie clară a fiecărei modificări, permițându-ți să vezi cine a făcut o anumită schimbare și de ce. În caz de erori sau conflicte, aceste informații te pot ajuta să înțelegi rapid ce s-a întâmplat și să revii la un punct anterior, dacă este necesar.

---

## Capitolul 3: Ramificări și Măsurarea Conflictului

### 3.1 Ramificări (Branches)

Ramificările (branches) sunt o caracteristică esențială în Git care permit dezvoltarea paralelă a funcționalităților, corectarea erorilor și experimentarea fără a afecta ramura principală (de obicei, numită `master` sau `main`). Când creezi o ramură nouă, creezi o copie separată a codului tău curent, pe care poți face modificări fără a influența ramura principală.

#### Crearea unei Ramuri Noi / Branch nou

Pentru a crea o ramură nouă și a trece la ea, folosește comanda:

```bash
git checkout -b nume-ramura
```

Aceasta creează și schimbă ramura curentă în ramura `nume-ramura`.

#### Combinarea Ramurilor (Branch Merging)

După ce ai terminat lucrul pe o ramură, este posibil să dorești să integrezi modificările în ramura principală. Pentru a face acest lucru, urmează acești pași:

1. **Schimbă la ramura principală**:
   ```bash
   git checkout master
   ```

2. **Integrează modificările**:
   ```bash
   git merge nume-ramura
   ```

Aceasta va adăuga modificările din `nume-ramura` în ramura `master`.

#### Rezolvarea Conflictelor

Uneori, când încerci să faci merge, este posibil să întâlnești conflicte dacă modificările de pe ramuri diferite se suprapun. Git va marca fișierele cu conflicte și va trebui să le rezolvi manual. După ce ai rezolvat conflictele, urmează acești pași:

1. **Adaugă fișierele modificate**:
   ```bash
   git add nume-fisier
   ```

2. **Finalizează merge-ul**:
   ```bash
   git commit
   ```

Aceasta finalizează merge-ul și include modificările rezolvate.

---

### 3.2 Recomandări pentru Utilizarea Ramurilor

- **Folosește ramuri pentru funcționalități noi**: Creează ramuri separate pentru fiecare funcționalitate nouă pe care o dezvolți. Acest lucru ajută la menținerea codului principal stabil și permite testarea și dezvoltarea funcționalităților noi în mod izolat.

- **Utilizează ramuri pentru corectarea erorilor**: Atunci când găsești o eroare în cod, creează o ramură de corectare a erorilor pentru a rezolva problema. După corectarea erorii, integrează ramura de corectare în ramura principală.

- **Menține ramurile actualizate**: Dacă lucrezi la o ramură pentru o perioadă lungă, asigură-te că o actualizezi frecvent cu modificările din ramura principală pentru a evita conflictele majore.

---

## Capitolul 4: Lucrul cu Repositories Remote

### 4.1 Configurarea unui Remote Repository

Pentru a lucra cu un repository remote, trebuie să adaugi un URL remote la repository-ul local. De obicei, acest URL este furnizat de platformele de hosting de cod, cum ar fi GitHub, GitLab sau Bitbucket.

#### Adăugarea unui Remote Repository

```bash
git remote add origin https://github.com/utilizator/nume-repo.git
```

Aceasta adaugă un repository remote denumit `origin`.

### 4.2 Împingerea și Tragerea Modificărilor

#### Împingerea Modificărilor

Pentru a trimite modificările tale către repository-ul remote, folosește comanda:

```bash
git push origin master
```

Aceasta trimite commit-urile din ramura locală `master` la ramura `master` din repository-ul remote `origin`.

#### Tragerea Modificărilor

Pentru a aduce ultimele modificări de la repository-ul remote, folosește comanda:

```bash
git pull origin master
```

Aceasta aduce modificările de la ramura `master` din `origin` și le integrează în ramura locală curentă.

### 4.3 Clonarea unui Repository

Dacă dorești să copiezi un repository remote pe computerul tău local, folosește comanda:

```bash
git clone https://github.com/utilizator/nume-repo.git
```

Aceasta creează o copie locală a repository-ului remote, inclusiv toate ramurile și istoricul commit-urilor.

---

## Capitolul 5: Tranzacții Avansate cu Git

### 5.1 Revertirea Modificărilor

Dacă dorești să anulezi modificările făcute într-un commit, poți folosi comanda `git revert`. Aceasta creează un nou commit care inversează modificările din commit-ul specificat.

```bash
git revert <commit-hash>
```

### 5.2 Resetarea Modificărilor

Pentru a elimina complet modificările dintr-un commit, poți folosi comanda `git reset`. Aceasta poate fi utilizată pentru a reseta indexul și starea de lucru la un anumit commit.

```bash
# Resetează indexul și starea de lucru la commit-ul specificat
git reset --hard <commit-hash>
```

**Atenție**: `git reset --hard` va șterge modificările necommite și poate duce la pierderea datelor.

### 5.3 Stash

Dacă lucrezi la o modificare, dar trebuie să schimbi temporar ramura sau să faci altceva, poți folosi comanda `git stash` pentru a salva modificările curente într-un stash temporar.

```bash
# Salvează modificările curente într-un stash
git stash

# Listă stash-urile disponibile
git stash list

# Aplică ultimul stash
git stash apply
```

---

## Capitolul 6: Practici Recomandate

### 6.1 Mesaje de Commit

Scrie mesaje de commit clare și descriptive. Mesajele ar trebui să explice ce a fost schimbat și de ce. De exemplu:

```bash
git commit -m "Adaugă funcționalitate de căutare în pagină"
```

### 6.2 Fă Commit-uri Frecvente

Fă commit-uri frecvente pentru a păstra un istoric detaliat al modificărilor. Acest lucru ajută la identificarea și remedierea problemelor mai ușor și permite colaborarea mai eficientă în echipe.

### 6.3 Revizuirea Codului

Revizuirea codului este esențială pentru a menține calitatea codului și pentru a identifica probleme înainte de integrarea modificărilor. Folosește pull requests (PR) și revizuiește codul altor dezvoltatori pentru a menține standardele de codare.

### 6.4 Branch naming (cum se denumesc branch-urile)

De fiecare data este bine sa creezi un name in stilul **KEBAB CASE** \
Care se traduce in felul urmator: \
Din \
**Mergem la munte si ne distram** \
in \
**mergem-la-munte-si-ne-distram**


git checkout -b mergem-la-munte-si-ne-distram // se creaza branch-ul \
git commit -m "mergem maine la munte sa ne distram" // comitem modificarile

### 6.5 Ce este .gitignore si ce trebuie inclus in el
Fișierul `.gitignore` este utilizat în sistemele de control al versiunilor, cum ar fi Git, pentru a specifica ce fișiere și directoare să fie ignorate de Git. Adică, fișierele și directoarele enumerate în acest fișier nu vor fi urmărite de Git, ceea ce înseamnă că nu vor fi incluse în commit-uri și nu vor apărea în istoricul versiunilor.

### **De ce să folosești un fișier `.gitignore`?**

1. **Reducerea zgomotului**: Fișierele generate automat, precum cele de configurare a IDE-urilor, fișierele de build sau cele de cache, nu sunt relevante pentru istoricul codului sursă și pot face ca istoricul să devină greu de gestionat.

2. **Protejarea datelor sensibile**: Fișierele care conțin informații sensibile sau de configurare (de exemplu, fișiere `.env` care conțin variabile de mediu) nu ar trebui să fie incluse în controlul versiunilor pentru a preveni expunerea lor accidentală.

3. **Îmbunătățirea performanței**: Ignorând fișierele inutile, Git lucrează mai eficient, iar operațiunile precum commit-urile și clonarea devin mai rapide.

### **Ce trebuie inclus în fișierul `.gitignore`?**

1. **Fișiere și directoare generate automat**:
    - Fișierele de build și directoarele, cum ar fi `dist/`, `build/`, `target/`.
    - Fișiere de log, cum ar fi `*.log`.

2. **Fișiere de configurare IDE**:
    - Fișierele generate de IDE-uri, cum ar fi `.idea/` (IntelliJ IDEA), `.vscode/` (Visual Studio Code), `*.iml`.

3. **Fișiere temporare și de sistem**:
    - Fișiere specifice sistemului de operare, cum ar fi `.DS_Store` (macOS), `Thumbs.db` (Windows).

4. **Fișiere de configurare personalizate**:
    - Fișiere care conțin informații sensibile sau configurări locale, cum ar fi `.env`, `config.php`.

5. **Dependențe externe**:
    - Directoare care conțin module externe, cum ar fi `node_modules/` (pentru proiectele Node.js) sau `vendor/` (pentru proiectele PHP cu Composer).

--- 

## Capitolul 7: Resurse Suplimentare

### 7.1 Documentație Oficială

- [Documentația Git](https://git-scm.com/doc)

### 7.2 Tutoriale și Cursuri

- [Tutorial Git de la Atlassian](https://www.atlassian.com/git/tutorials)
- [GitHub Learning Lab](https://lab.github.com/)

### 7.3 Comunități și Forumuri

- [Stack Overflow](https://stackoverflow.com/questions/tagged/git)
- [GitHub Discussions](https://github.com/github/community-discussions)


---
