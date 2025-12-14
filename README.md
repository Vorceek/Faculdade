# 📋 CRUD de Funcionários – Django

## 📌 Descrição do Projeto

Este projeto consiste no desenvolvimento de um **CRUD (Create, Read, Update e Delete)** para **Funcionários**, utilizando o framework **Django**, banco de dados **MySQL** e **Bootstrap** para estilização das páginas.

O projeto foi desenvolvido seguindo **rigorosamente o passo a passo apresentado em aula**, conforme solicitado na **Atividade Avaliativa 3**, contemplando todas as funcionalidades exigidas.

---

## 🛠️ Tecnologias Utilizadas

- Python  
- Django  
- MySQL  
- django-bootstrap5  
- HTML5  
- Bootstrap  

---

## 📁 Estrutura do Projeto

```
atividade-crud/
│
├── app/
│   ├── migrations/
│   ├── templates/
│   │   ├── form_funcionario.html
│   │   ├── lista_funcionarios.html
│   │   ├── lista_funcionario.html
│   │   └── remover_funcionario.html
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   └── tests.py
│
├── funcionario/
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── venv/
├── manage.py
└── README.md
```

---

## ⚙️ Configuração do Ambiente

### 1️⃣ Criar e ativar o ambiente virtual

```bash
virtualenv venv
venv\Scripts\activate
```

---

### 2️⃣ Instalar as dependências

```bash
pip install django
pip install mysqlclient
pip install django-bootstrap5
```

---

### 3️⃣ Criar o banco de dados

```sql
CREATE DATABASE funcionarios;
```

---

### 4️⃣ Configurar o banco no `settings.py`

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'HOST': 'localhost',
        'PORT': '3306',
        'USER': 'root',
        'PASSWORD': 'root',
        'NAME': 'funcionarios',
    }
}
```

---

## ▶️ Executando o Projeto

```bash
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
```

Acesse:
```
http://localhost:8000
```

---

## 🔄 Funcionalidades do CRUD

### ➕ Cadastrar Funcionário
`/app/form_funcionario`

### 📄 Listar Funcionários
`/app/lista_funcionarios`

### ✏️ Editar Funcionário
`/app/form_funcionario/<id>`

### 🔍 Visualizar Funcionário
`/app/lista_funcionario/<id>`

### ❌ Remover Funcionário
`/app/remover_funcionario/<id>`

---

## 🎨 Estilização

- Bootstrap
- Tabelas com `table-striped`
- Botões estilizados
- Margem aplicada via CSS

---

## 📚 Referências

- https://docs.djangoproject.com/
- https://getbootstrap.com/
- https://www.w3schools.com/
