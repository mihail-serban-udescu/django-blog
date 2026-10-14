# Blog Django

Un blog complet dezvoltat cu **Django 6.1** și **Bootstrap 5**, cu sistem de autentificare, CRUD pentru postări, comentarii, căutare și paginare.

## 🚀 Features

- ✅ **CRUD complet** pentru postări (Create, Read, Update, Delete)
- ✅ **Sistem de comentarii** cu moderare
- ✅ **Autentificare utilizatori** (login/logout)
- ✅ **Permisiuni** — doar autorul poate edita/șterge propria postare
- ✅ **Categorii** de postări
- ✅ **Upload imagini** pentru postări (Pillow)
- ✅ **Căutare** în titlu și conținut
- ✅ **Paginare** (5 postări/pagină)
- ✅ **URL-uri cu slug** (SEO-friendly)
- ✅ **Admin panel** customizat
- ✅ **Design responsive** cu Bootstrap 5

## 🛠️ Tehnologii

- **Python 3.12**
- **Django 6.1**
- **SQLite** (dev) — ușor de schimbat cu PostgreSQL
- **Bootstrap 5** + Bootstrap Icons
- **Pillow** (procesare imagini)

## 📦 Instalare

### 1. Clonează repository-ul

```bash
git clone https://github.com/mihail-serban-udescu/django-blog.git
cd django-blog
2. Creează virtual environment
bash
python -m venv venv

# Windows
venv\Scripts\activate

# Linux/Mac
source venv/bin/activate
3. Instalează dependențele
bash
pip install -r requirements.txt
4. Aplică migrațiile
bash
python manage.py migrate
5. Creează superuser
bash
python manage.py createsuperuser
6. Pornește serverul
bash
python manage.py runserver
Deschide browserul la: http://127.0.0.1:8000/blog/

📖 Utilizare
Admin panel: http://127.0.0.1:8000/admin/

Blog: http://127.0.0.1:8000/blog/

Login: http://127.0.0.1:8000/accounts/login/

📸 Screenshots
Lista postărilor
https://screenshots/post_list.png

Detaliu postare cu comentarii
https://screenshots/post_detail.png

Admin panel
https://screenshots/admin.png

🏗️ Structura proiectului
text
django-blog/
├── blog/
│   ├── migrations/
│   ├── templates/blog/
│   │   ├── base.html
│   │   ├── post_list.html
│   │   ├── post_detail.html
│   │   ├── post_form.html
│   │   └── post_confirm_delete.html
│   ├── admin.py
│   ├── forms.py
│   ├── models.py
│   ├── urls.py
│   └── views.py
├── blog_project/
│   ├── settings.py
│   └── urls.py
├── templates/registration/
│   └── login.html
├── media/
├── manage.py
├── requirements.txt
└── README.md
🧪 Modele
Category — categorii de postări

Post — articole cu slug, autor, categorie, imagine, status

Comment — comentarii legate de post și user

📝 Licență
Proiect personal de portofoliu — Mihail, 2026.
