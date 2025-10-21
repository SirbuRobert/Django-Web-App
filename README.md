# Django Web App

O aplicație web construită cu Django — un proiect simplu de magazin/producte (album‑shop) pentru scopuri de învățare/prototip.

## Cuprins

- [Descriere](#descriere)  
- [Funcționalități](#funcționalități)  
- [Tehnologii](#tehnologii)  
- [Instalare & configurare locală](#instalare--configurare‑locală)  
- [Structură proiect](#structură‑proiect)  
- [Utilizare](#utilizare)  
- [Contribuții](#contribuții)  
- [Licență](#licență)  
- [Contact](#contact)  

---

## Descriere  
Această aplicație este un magazin online simplu, construit cu Django, care permite vizualizarea produselor (albume), navigarea în magazin şi un panou administrativ.  
Scopul principal este de a învăţa şi explora Django în practică.

---

## Funcționalități  
- Pagina principală a magazinului (ex: `http://127.0.0.1:8000/magazin/albume`) pentru vizualizarea produselor.  
- Formular de autentificare / super‑user (via `createsuperuser`) pentru acces în zona administrativă.  
- Panou admin Django (via `http://127.0.0.1:8000/admin`) pentru gestionarea produselor/îmachetărilor.  
- Gestionare fişiere statice, media şi template‑uri personalizate.  

---

## Tehnologii  
- Django (Python)  
- HTML, CSS, JavaScript  
- Structură de proiect Django standard (apps, templates, static, media)  
- (Opţional) Baza de date SQLite pentru dezvoltare locală  

---

## Instalare & configurare locală  
Urmează paşii de mai jos pentru a rula aplicaţia local:

1. Clonează repo‑ul:
   ```bash
   git clone https://github.com/SirbuRobert/Django‑Web‑App.git
   cd Django‑Web‑App
   ```
2. Creează (opţional) un mediu virtual Python:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # pe Linux/macOS
   venv\Scripts\activate     # pe Windows
   ```
3. Instalează dependenţele (dacă ai un fişier `requirements.txt`; dacă nu, instalează Django manual):
   ```bash
   pip install django
   # pip install -r requirements.txt
   ```
4. Aplică migraţiile:
   ```bash
   python manage.py migrate
   ```
5. Creează un super‑user:
   ```bash
   python manage.py createsuperuser
   ```
6. Rulează serverul de dezvoltare:
   ```bash
   python manage.py runserver
   ```
7. Deschide în browser:
   - Magazin: http://127.0.0.1:8000/magazin/albume  
   - Admin:  http://127.0.0.1:8000/admin  

---

## Structură proiect  
```
Django‑Web‑App/
├── magazin/             # aplicaţia principală „magazin”
├── media/               # fişiere uploadate (ex: imagini produse)
├── proiect/             # proiectul Django (setări, urls etc.)
├── static/              # fişiere statice (CSS, JS, imagini)
├── templates/           # template‑uri HTML
├── manage.py
└── README.md
```

---

## Utilizare  
- Navighează la pagina magazinului pentru a vedea lista de albume.  
- Autentifică‑te în panoul admin pentru a adăuga/edita/elimina produse.  
- Poţi adapta aplicaţia la alte tipuri de produse sau extinde funcţionalităţile: filtrare, căutare, coş de cumpărături etc.


*Acest README a fost generat automat şi poate fi personalizat după nevoi.*
