# MeviMensager 🚀

Um clone do WhatsApp acessível via navegador e aplicativo mobile, usando:

- **Backend**: Django + Django REST Framework
- **Frontend Web**: React.js
- **Mobile**: Flutter
- **Banco de dados**: SQL (SQLite em desenvolvimento)

---

## 🎯 Funcionalidades

- Login com conta Google e email
- Envio de mensagens
- Acesso via Web ou Aplicativo
- Armazenamento temporário de mensagens

---

## 🛠️ Como rodar localmente

### Backend (Django)
```bash
cd backend
python -m venv venv
source venv/bin/activate (Linux/Mac) ou venv\Scripts\activate (Windows)
pip install -r requirements.txt
python manage.py runserver
