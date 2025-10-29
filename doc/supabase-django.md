⚙️ Passo a passo para conectar o Django ao Supabase
1️⃣ Obtenha os dados de conexão do Supabase

No painel do Supabase → Settings → Database

Host
Port
Database
User
Password

2️⃣ Configure o settings.py do Django

* No seu projeto Django (ecommerce/settings.py), altere a parte do banco de dados:
```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'postgres',  # nome do banco (normalmente "postgres" por padrão)
        'USER': 'postgres',  # seu usuário Supabase
        'PASSWORD': 'sua_senha_aqui',
        'HOST': 'db.xxxxx.supabase.co',  # host do Supabase
        'PORT': '5432',
    }
}
```

3️⃣ migration
```
python manage.py makemigrations
python manage.py migrate
```


4️⃣ teste
```
python manage.py dbshell
```

🔧 Talvez precise instalar o driver:
```
pip install psycopg2-binary
```

