# <span style="color:darkpurple;">TOTUL DESPRE GIT</span>


## <span style="color:darkpurple;">Capitolul 1: Introducere în Git și Sistemele de Control al Versiunilor</span>

### <span style="color:darkpurple;">Capitolul 1: Introducere în Git</span>

### <span style="color:darkpurple;">1.1 Ce este Git?</span>
- Definiție și scop
- Istoricul și dezvoltarea Git

### <span style="color:darkpurple;">1.2 Instalarea Git</span>
- Instalarea pe Windows
- Instalarea pe macOS
- Instalarea pe Linux

### <span style="color:darkpurple;">1.3 Configurarea Git</span>
- Configurarea numelui și a e-mailului
- Alte setări de bază

## <span style="color:darkpurple;">Capitolul 2: Concepte de Bază în Git</span>

### <span style="color:darkpurple;">2.1 Repositories</span>
- Definiție și scop
- Tipuri de repository-uri (local și remote)
- Inițializarea unui repository local

### <span style="color:darkpurple;">2.2 Staging și Commiting</span>
- Stările fișierelor (untracked, staged, modified)
- Procesul de adăugare și commit
    - Comanda <span style="color:darkorange;">git add</span>
    - Comanda <span style="color:darkorange;">git commit</span>
- Comentarii în cod pentru fiecare pas al procesului

### <span style="color:darkpurple;">2.3 Vizualizarea Istoricului</span>
- Comanda <span style="color:darkorange;">git log</span>
- Interpretarea rezultatelor și utilizarea istoricului

## <span style="color:darkpurple;">Capitolul 3: Ramificări și Măsurarea Conflictului</span>

### <span style="color:darkpurple;">3.1 Ramificări (Branches)</span>
- Definiție și utilizare
- Crearea unei ramuri noi
    - Comanda <span style="color:darkorange;">git checkout -b</span>
- Combinarea ramurilor (merging)
    - Comanda <span style="color:darkorange;">git merge</span>
- Rezolvarea conflictelor
    - Procesul și comenzi pentru rezolvarea conflictelor

### <span style="color:darkpurple;">3.2 Recomandări pentru Utilizarea Ramurilor</span>
- Folosirea ramurilor pentru funcționalități noi și corectarea erorilor
- Menținerea ramurilor actualizate

## <span style="color:darkpurple;">Capitolul 4: Lucrul cu Repositories Remote</span>

### <span style="color:darkpurple;">4.1 Configurarea unui Remote Repository</span>
- Adăugarea unui remote repository
    - Comanda <span style="color:darkorange;">git remote add</span>

### <span style="color:darkpurple;">4.2 Împingerea și Tragerea Modificărilor</span>
- Împingerea modificărilor
    - Comanda <span style="color:darkorange;">git push</span>
- Tragerea modificărilor
    - Comanda <span style="color:darkorange;">git pull</span>

### <span style="color:darkpurple;">4.3 Clonarea unui Repository</span>
- Comanda <span style="color:darkorange;">git clone</span>
- Utilizarea repository-ului clonat

## <span style="color:darkpurple;">Capitolul 5: Tranzacții Avansate cu Git</span>

### <span style="color:darkpurple;">5.1 Revertirea Modificărilor</span>
- Utilizarea comenzii <span style="color:darkorange;">git revert</span>
- Exemple de revertire a modificărilor

### <span style="color:darkpurple;">5.2 Resetarea Modificărilor</span>
- Utilizarea comenzii <span style="color:darkorange;">git reset</span>
- Diferența între resetare soft și hard

### <span style="color:darkpurple;">5.3 Stash</span>
- Utilizarea comenzii <span style="color:darkorange;">git stash</span>
- Aplicarea și gestionarea stash-urilor

## <span style="color:darkpurple;">Capitolul 6: Practici Recomandate</span>

### <span style="color:darkpurple;">6.1 Mesaje de Commit</span>
- Scrierea mesajelor de commit clare și descriptive

### <span style="color:darkpurple;">6.2 Fă Commit-uri Frecvente</span>
- Importanța commit-urilor frecvente

### <span style="color:darkpurple;">6.3 Revizuirea Codului</span>
- Utilizarea pull requests (PR) pentru revizuirea codului
- Importanța revizuirii codului pentru menținerea calității

## <span style="color:darkpurple;">Capitolul 7: Resurse Suplimentare</span>

### <span style="color:darkpurple;">7.1 Documentație Oficială</span>
- Link-uri și resurse pentru documentația oficială Git

### <span style="color:darkpurple;">7.2 Tutoriale și Cursuri</span>
- Link-uri către tutoriale și cursuri online

### <span style="color:darkpurple;">7.3 Comunități și Forumuri</span>
- Link-uri către comunități și forumuri de suport

## <span style="color:darkpurple;">Anexe</span>
- Ghid rapid de comenzi Git esențiale.
- Exemple de <span style="color:darkorange;">.gitignore</span> pentru diverse tipuri de proiecte.
- Exemple de workflow-uri Git într-un mediu colaborativ.

# <span style="color:darkpurple;">**Curs Git: Ghid Practic pentru Începători**</span>

## <span style="color:darkpurple;">Capitolul 1: Introducere în Git</span>

### <span style="color:darkpurple;">1.1 Ce este Git?</span>

Git este un sistem de control al versiunilor distribuit, utilizat pentru a urmări modificările aduse fișierelor într-un proiect. Permite colaborarea eficientă între mai mulți dezvoltatori, oferind funcționalități avansate pentru gestionarea istoricelor de modificări și a ramificărilor codului.

Git a fost creat de Linus Torvalds în 2005 pentru a sprijini dezvoltarea kernelului Linux. De-a lungul timpului, Git a devenit un instrument esențial în dezvoltarea software-ului, folosit de echipe de toate dimensiunile pentru a gestiona codul sursă și a coordona activitățile dezvoltatorilor.

### <span style="color:darkpurple;">1.2 Instalarea Git</span>

Pentru a începe să folosești Git, trebuie să îl instalezi pe sistemul tău. Pașii pentru instalare variază în funcție de sistemul de operare.

#### <span style="color:darkpurple;">Pe Windows:</span>
1. Descarcă Git de la [site-ul oficial](https://git-scm.com/downloads).
2. Rulați installerul și urmați instrucțiunile pentru a finaliza instalarea.

#### <span style="color:darkpurple;">Pe macOS:</span>
1. Deschideți Terminalul.
2. Folosiți Homebrew pentru a instala Git: <span style="color:darkorange;">brew install git</span>.

#### <span style="color:darkpurple;">Pe Linux:</span>
1. Deschideți terminalul.
2. Utilizați managerul de pachete al distribuției dvs. pentru a instala Git. De exemplu, pe Ubuntu: <span style="color:darkorange;">sudo apt-get install git</span>.

### <span style="color:darkpurple;">1.3 Configurarea Git</span>

După instalare, este important să configurezi Git cu informațiile tale de utilizator. Aceste setări vor fi incluse în commit-urile tale pentru a le asocia cu numele și adresa ta de e-mail.

``<span style="color:darkorange;">bash
# <span style="color:darkpurple;">Configurare nume și e-mail</span>
git config --global user.name "Numele Tău"
git config --global user.email "emailul@tau.com"
</span>`<span style="color:darkorange;">

Aceste comenzi setează informațiile de bază care vor fi incluse în fiecare commit pe care îl faci.

---

## <span style="color:darkpurple;">Capitolul 2: Concepte de Bază în Git</span>

### <span style="color:darkpurple;">2.1 Repositories</span>

Un repository (sau repo) este locul unde Git stochează toate fișierele și istoricul de modificări ale unui proiect. Există două tipuri principale de repository-uri:

- **Local Repository**: Se află pe computerul tău local.
- **Remote Repository**: Este găzduit pe un server la distanță, de obicei pe platforme precum GitHub, GitLab sau Bitbucket.

Pentru a iniția un repository local, folosești comanda:

</span>`<span style="color:darkorange;">bash
git init
</span>`<span style="color:darkorange;">

Această comandă creează un nou repository Git în directorul curent.

---

### <span style="color:darkpurple;">2.2 Staging și Commiting</span>

Fișierele tale pot trece prin mai multe stări în Git. Imaginează-ți că lucrezi la un proiect de dezvoltare a unui site web. Tocmai ce ai creat o nouă pagină HTML pentru secțiunea de "Contact" și vrei să adaugi modificările în Git. În acel moment, fișierul este în starea de **untracked**, ceea ce înseamnă că Git încă nu îl urmărește.

După ce decizi să-l adaugi în Git folosind comanda </span>git add<span style="color:darkorange;">, fișierul intră în starea de **staged**, adică este pregătit pentru a fi confirmat într-un commit. Ulterior, dacă faci modificări pe acest fișier, el va intra în starea de **modified**, indicând că există schimbări care nu au fost încă salvate într-un commit. Acest ciclu al stărilor fișierelor te ajută să urmărești fiecare etapă a dezvoltării.

Să presupunem că tocmai ai creat un fișier </span>contact.html<span style="color:darkorange;"> pentru secțiunea de "Contact" a unui site. Procesul ar putea arăta astfel:

</span>`<span style="color:darkorange;">bash
# <span style="color:darkpurple;">Creăm noul fișier HTML pentru pagina de contact</span>
touch contact.html

# <span style="color:darkpurple;">Verificăm starea fișierelor în Git. "contact.html" apare ca untracked.</span>
git status
# <span style="color:darkpurple;">Output:</span>
# <span style="color:darkpurple;">Untracked files:</span>
# <span style="color:darkpurple;">  (use "git add <file>..." to include in what will be committed)</span>
# <span style="color:darkpurple;">        contact.html</span>

# <span style="color:darkpurple;">Adăugăm fișierul în zona de staging, pregătindu-l pentru un commit</span>
git add contact.html

# <span style="color:darkpurple;">Verificăm din nou starea. Acum fișierul "contact.html" este în staging.</span>
git status
# <span style="color:darkpurple;">Output:</span>
# <span style="color:darkpurple;">Changes to be committed:</span>
# <span style="color:darkpurple;">  (use "git restore --staged <file>..." to unstage)</span>
# <span style="color:darkpurple;">        new file:   contact.html</span>

# <span style="color:darkpurple;">Facem un commit cu un mesaj care explică adăugarea noii pagini</span>
git commit -m "Adaugă pagina de contact"
# <span style="color:darkpurple;">Output:</span>
# <span style="color:darkpurple;">[master 123abc] Adaugă pagina de contact</span>
# <span style="color:darkpurple;"> 1 file changed, 0 insertions(+), 0 deletions(+)</span>
# <span style="color:darkpurple;"> create mode 100644 contact.html</span>
</span>`<span style="color:darkorange;">

#### <span style="color:darkpurple;">Pasi de urmat</span>

</span>`<span style="color:darkorange;">bash
# <span style="color:darkpurple;">Pasul 1: "touch contact.html" creează un fișier gol numit contact.html.</span>
# <span style="color:darkpurple;">La acest punct, fișierul este în starea de "untracked", ceea ce înseamnă că Git încă nu îl monitorizează.</span>
# <span style="color:darkpurple;">Pasul 2: "git status" ne arată că fișierul contact.html este untracked.</span>
# <span style="color:darkpurple;">Pasul 3: "git add contact.html" adaugă fișierul în zona de staging, unde Git îl pregătește pentru un commit.</span>
# <span style="color:darkpurple;">Pasul 4: "git status" arată că fișierul este acum în starea "staged", gata să fie confirmat.</span>
# <span style="color:darkpurple;">Pasul 5: "git commit -m 'Adaugă pagina de contact'" creează un commit, care salvează modificările făcute.</span>
</span>`<span style="color:darkorange;">

Acest proces este utilizat zilnic de dezvoltatori care lucrează la proiecte mari sau mici. Fiecare fișier nou creat într-un proiect trebuie să fie adăugat în Git pentru a fi urmărit. De exemplu, atunci când lucrezi la un site și creezi o nouă pagină sau un fișier CSS, acest fișier va trece prin etapele **untracked**, **staged**, și eventual **committed**. În acest fel, poți păstra un istoric detaliat al fiecărei modificări și poți colabora eficient cu echipa ta.

---

### <span style="color:darkpurple;">2.3 Vizualizarea Istoricului</span>

Git păstrează un istoric detaliat al tuturor commit-urilor efectuate. Comanda </span>git log<span style="color:darkorange;"> este folosită pentru a vizualiza acest istoric, oferind informații despre fiecare commit, inclusiv mesajul acestuia, autorul și data.

</span>`<span style="color:darkorange;">bash
git log
# <span style="color:darkpurple;">Output (exemplu):</span>
# <span style="color:darkpurple;">commit 94f1e28393a4bc6a45d4a2a9d81e87f857b3b3f4 (HEAD -> master)</span>
# <span style="color:darkpurple;">Author: Nume Utilizator <emailul@tau.com></span>
# <span style="color:darkpurple;">Date:   Fri Sep 6 12:34:56 2023 +0300</span>
#
# <span style="color:darkpurple;">    Adaugă pagina principală index.html</span>
</span>`<span style="color:darkorange;">

#### <span style="color:darkpurple;">Pasi de urmat</span>

</span>`<span style="color:darkorange;">bash
# <span style="color:darkpurple;">Pasul 1: "git log" afișează commit-urile recente, împreună cu autorul, data și mesajul descriptiv.</span>
# <span style="color:darkpurple;">Pasul 2: Fiecare commit conține un hash unic, care este identificatorul acelui commit.</span>
# <span style="color:darkpurple;">Pasul 3: Autorul commit-ului și data oferă informații despre cine și când a făcut schimbările.</span>
# <span style="color:darkpurple;">Pasul 4: Mesajul commit-ului explică clar ce a fost schimbat sau adăugat în cadrul acelui commit.</span>
</span>`<span style="color:darkorange;">

Această practică este extrem de utilă atunci când lucrezi într-o echipă de dezvoltare. Istoricul commit-urilor oferă o cronologie clară a fiecărei modificări, permițându-ți să vezi cine a făcut o anumită schimbare și de ce. În caz de erori sau conflicte, aceste informații te pot ajuta să înțelegi rapid ce s-a întâmplat și să revii la un punct anterior, dacă este necesar.

---

## <span style="color:darkpurple;">Capitolul 3: Ramificări și Măsurarea Conflictului</span>

### <span style="color:darkpurple;">3.1 Ramificări (Branches)</span>

Ramificările (branches) sunt o caracteristică esențială în Git care permit dezvoltarea paralelă a funcționalităților, corectarea erorilor și experimentarea fără a afecta ramura principală (de obicei, numită </span>master<span style="color:darkorange;"> sau </span>main<span style="color:darkorange;">). Când creezi o ramură nouă, creezi o copie separată a codului tău curent, pe care poți face modificări fără a influența ramura principală.

#### <span style="color:darkpurple;">Crearea unei Ramuri Noi / Branch nou</span>

Pentru a crea o ramură nouă și a trece la ea, folosește comanda:

</span>`<span style="color:darkorange;">bash
git checkout -b nume-ramura
</span>`<span style="color:darkorange;">

Aceasta creează și schimbă ramura curentă în ramura </span>nume-ramura<span style="color:darkorange;">.

#### <span style="color:darkpurple;">Combinarea Ramurilor (Branch Merging)</span>

După ce ai terminat lucrul pe o ramură, este posibil să dorești să integrezi modificările în ramura principală. Pentru a face acest lucru, urmează acești pași:

1. **Schimbă la ramura principală**:
   </span>`<span style="color:darkorange;">bash
   git checkout master
   </span>`<span style="color:darkorange;">

2. **Integrează modificările**:
   </span>`<span style="color:darkorange;">bash
   git merge nume-ramura
   </span>`<span style="color:darkorange;">

Aceasta va adăuga modificările din </span>nume-ramura<span style="color:darkorange;"> în ramura </span>master<span style="color:darkorange;">.

#### <span style="color:darkpurple;">Rezolvarea Conflictelor</span>

Uneori, când încerci să faci merge, este posibil să întâlnești conflicte dacă modificările de pe ramuri diferite se suprapun. Git va marca fișierele cu conflicte și va trebui să le rezolvi manual. După ce ai rezolvat conflictele, urmează acești pași:

1. **Adaugă fișierele modificate**:
   </span>`<span style="color:darkorange;">bash
   git add nume-fisier
   </span>`<span style="color:darkorange;">

2. **Finalizează merge-ul**:
   </span>`<span style="color:darkorange;">bash
   git commit
   </span>`<span style="color:darkorange;">

Aceasta finalizează merge-ul și include modificările rezolvate.

---

### <span style="color:darkpurple;">3.2 Recomandări pentru Utilizarea Ramurilor</span>

- **Folosește ramuri pentru funcționalități noi**: Creează ramuri separate pentru fiecare funcționalitate nouă pe care o dezvolți. Acest lucru ajută la menținerea codului principal stabil și permite testarea și dezvoltarea funcționalităților noi în mod izolat.

- **Utilizează ramuri pentru corectarea erorilor**: Atunci când găsești o eroare în cod, creează o ramură de corectare a erorilor pentru a rezolva problema. După corectarea erorii, integrează ramura de corectare în ramura principală.

- **Menține ramurile actualizate**: Dacă lucrezi la o ramură pentru o perioadă lungă, asigură-te că o actualizezi frecvent cu modificările din ramura principală pentru a evita conflictele majore.

---

## <span style="color:darkpurple;">Capitolul 4: Lucrul cu Repositories Remote</span>

### <span style="color:darkpurple;">4.1 Configurarea unui Remote Repository</span>

Pentru a lucra cu un repository remote, trebuie să adaugi un URL remote la repository-ul local. De obicei, acest URL este furnizat de platformele de hosting de cod, cum ar fi GitHub, GitLab sau Bitbucket.

#### <span style="color:darkpurple;">Adăugarea unui Remote Repository</span>

</span>`<span style="color:darkorange;">bash
git remote add origin https://github.com/utilizator/nume-repo.git
</span>`<span style="color:darkorange;">

Aceasta adaugă un repository remote denumit </span>origin<span style="color:darkorange;">.

### <span style="color:darkpurple;">4.2 Împingerea și Tragerea Modificărilor</span>

#### <span style="color:darkpurple;">Împingerea Modificărilor</span>

Pentru a trimite modificările tale către repository-ul remote, folosește comanda:

</span>`<span style="color:darkorange;">bash
git push origin master
</span>`<span style="color:darkorange;">

Aceasta trimite commit-urile din ramura locală </span>master<span style="color:darkorange;"> la ramura </span>master<span style="color:darkorange;"> din repository-ul remote </span>origin<span style="color:darkorange;">.

#### <span style="color:darkpurple;">Tragerea Modificărilor</span>

Pentru a aduce ultimele modificări de la repository-ul remote, folosește comanda:

</span>`<span style="color:darkorange;">bash
git pull origin master
</span>`<span style="color:darkorange;">

Aceasta aduce modificările de la ramura </span>master<span style="color:darkorange;"> din </span>origin<span style="color:darkorange;"> și le integrează în ramura locală curentă.

### <span style="color:darkpurple;">4.3 Clonarea unui Repository</span>

Dacă dorești să copiezi un repository remote pe computerul tău local, folosește comanda:

</span>`<span style="color:darkorange;">bash
git clone https://github.com/utilizator/nume-repo.git
</span>`<span style="color:darkorange;">

Aceasta creează o copie locală a repository-ului remote, inclusiv toate ramurile și istoricul commit-urilor.

---

## <span style="color:darkpurple;">Capitolul 5: Tranzacții Avansate cu Git</span>

### <span style="color:darkpurple;">5.1 Revertirea Modificărilor</span>

Dacă dorești să anulezi modificările făcute într-un commit, poți folosi comanda </span>git revert<span style="color:darkorange;">. Aceasta creează un nou commit care inversează modificările din commit-ul specificat.

</span>`<span style="color:darkorange;">bash
git revert <commit-hash>
</span>`<span style="color:darkorange;">

### <span style="color:darkpurple;">5.2 Resetarea Modificărilor</span>

Pentru a elimina complet modificările dintr-un commit, poți folosi comanda </span>git reset<span style="color:darkorange;">. Aceasta poate fi utilizată pentru a reseta indexul și starea de lucru la un anumit commit.

</span>`<span style="color:darkorange;">bash
# <span style="color:darkpurple;">Resetează indexul și starea de lucru la commit-ul specificat</span>
git reset --hard <commit-hash>
</span>`<span style="color:darkorange;">

**Atenție**: </span>git reset --hard<span style="color:darkorange;"> va șterge modificările necommite și poate duce la pierderea datelor.

### <span style="color:darkpurple;">5.3 Stash</span>

Dacă lucrezi la o modificare, dar trebuie să schimbi temporar ramura sau să faci altceva, poți folosi comanda </span>git stash<span style="color:darkorange;"> pentru a salva modificările curente într-un stash temporar.

</span>`<span style="color:darkorange;">bash
# <span style="color:darkpurple;">Salvează modificările curente într-un stash</span>
git stash

# <span style="color:darkpurple;">Listă stash-urile disponibile</span>
git stash list

# <span style="color:darkpurple;">Aplică ultimul stash</span>
git stash apply
</span>`<span style="color:darkorange;">

---

## <span style="color:darkpurple;">Capitolul 6: Practici Recomandate</span>

### <span style="color:darkpurple;">6.1 Mesaje de Commit</span>

Scrie mesaje de commit clare și descriptive. Mesajele ar trebui să explice ce a fost schimbat și de ce. De exemplu:

</span>`<span style="color:darkorange;">bash
git commit -m "Adaugă funcționalitate de căutare în pagină"
</span>`<span style="color:darkorange;">

### <span style="color:darkpurple;">6.2 Fă Commit-uri Frecvente</span>

Fă commit-uri frecvente pentru a păstra un istoric detaliat al modificărilor. Acest lucru ajută la identificarea și remedierea problemelor mai ușor și permite colaborarea mai eficientă în echipe.

### <span style="color:darkpurple;">6.3 Revizuirea Codului</span>

Revizuirea codului este esențială pentru a menține calitatea codului și pentru a identifica probleme înainte de integrarea modificărilor. Folosește pull requests (PR) și revizuiește codul altor dezvoltatori pentru a menține standardele de codare.

### <span style="color:darkpurple;">6.4 Branch naming (cum se denumesc branch-urile)</span>

De fiecare data este bine sa creezi un name in stilul **KEBAB CASE** \
Care se traduce in felul urmator: \
Din \
**Mergem la munte si ne distram** \
in \
**mergem-la-munte-si-ne-distram**


git checkout -b mergem-la-munte-si-ne-distram // se creaza branch-ul \
git commit -m "mergem maine la munte sa ne distram" // comitem modificarile

### <span style="color:darkpurple;">6.5 Ce este .gitignore si ce trebuie inclus in el</span>
Fișierul </span>.gitignore<span style="color:darkorange;"> este utilizat în sistemele de control al versiunilor, cum ar fi Git, pentru a specifica ce fișiere și directoare să fie ignorate de Git. Adică, fișierele și directoarele enumerate în acest fișier nu vor fi urmărite de Git, ceea ce înseamnă că nu vor fi incluse în commit-uri și nu vor apărea în istoricul versiunilor.

### <span style="color:darkpurple;">**De ce să folosești un fișier </span>.gitignore<span style="color:darkorange;">?**</span>

1. **Reducerea zgomotului**: Fișierele generate automat, precum cele de configurare a IDE-urilor, fișierele de build sau cele de cache, nu sunt relevante pentru istoricul codului sursă și pot face ca istoricul să devină greu de gestionat.

2. **Protejarea datelor sensibile**: Fișierele care conțin informații sensibile sau de configurare (de exemplu, fișiere </span>.env<span style="color:darkorange;"> care conțin variabile de mediu) nu ar trebui să fie incluse în controlul versiunilor pentru a preveni expunerea lor accidentală.

3. **Îmbunătățirea performanței**: Ignorând fișierele inutile, Git lucrează mai eficient, iar operațiunile precum commit-urile și clonarea devin mai rapide.

### <span style="color:darkpurple;">**Ce trebuie inclus în fișierul </span>.gitignore<span style="color:darkorange;">?**</span>

1. **Fișiere și directoare generate automat**:
    - Fișierele de build și directoarele, cum ar fi </span>dist/<span style="color:darkorange;">, </span>build/<span style="color:darkorange;">, </span>target/<span style="color:darkorange;">.
    - Fișiere de log, cum ar fi </span>*.log<span style="color:darkorange;">.

2. **Fișiere de configurare IDE**:
    - Fișierele generate de IDE-uri, cum ar fi </span>.idea/<span style="color:darkorange;"> (IntelliJ IDEA), </span>.vscode/<span style="color:darkorange;"> (Visual Studio Code), </span>*.iml<span style="color:darkorange;">.

3. **Fișiere temporare și de sistem**:
    - Fișiere specifice sistemului de operare, cum ar fi </span>.DS_Store<span style="color:darkorange;"> (macOS), </span>Thumbs.db<span style="color:darkorange;"> (Windows).

4. **Fișiere de configurare personalizate**:
    - Fișiere care conțin informații sensibile sau configurări locale, cum ar fi </span>.env<span style="color:darkorange;">, </span>config.php<span style="color:darkorange;">.

5. **Dependențe externe**:
    - Directoare care conțin module externe, cum ar fi </span>node_modules/<span style="color:darkorange;"> (pentru proiectele Node.js) sau </span>vendor/` (pentru proiectele PHP cu Composer).

--- 

## <span style="color:darkpurple;">Capitolul 7: Resurse Suplimentare</span>

### <span style="color:darkpurple;">7.1 Documentație Oficială</span>

- [Documentația Git](https://git-scm.com/doc)

### <span style="color:darkpurple;">7.2 Tutoriale și Cursuri</span>

- [Tutorial Git de la Atlassian](https://www.atlassian.com/git/tutorials)
- [GitHub Learning Lab](https://lab.github.com/)

### <span style="color:darkpurple;">7.3 Comunități și Forumuri</span>

- [Stack Overflow](https://stackoverflow.com/questions/tagged/git)
- [GitHub Discussions](https://github.com/github/community-discussions)


---
