# 🐍💻 Comandos Essenciais do Django

> Guia rápido e visual dos **10 comandos mais usados** no framework **Django** — ideal para iniciantes e treinamentos práticos.

## 🚀 1. Criar um novo projeto


django-admin startproject nome_do_projeto


📁 Cria a estrutura base do seu projeto Django (com settings.py, urls.py, etc).

🧩 2. Criar um novo app
python manage.py startapp nome_do_app


📦 Cada app é um módulo independente (ex: usuarios, produtos, blog).

🖥️ 3. Rodar o servidor local
python manage.py runserver


🌐 Inicia o servidor de desenvolvimento (acesso padrão: http://127.0.0.1:8000
).

🧱 4. Criar migrações
python manage.py makemigrations


📜 Gera arquivos de migração com base nas alterações dos modelos (models.py).

🔁 5. Aplicar migrações ao banco
python manage.py migrate


🗃️ Executa as migrações e atualiza o banco de dados conforme os modelos definidos.

👑 6. Criar usuário administrador
python manage.py createsuperuser


🔐 Cria um usuário para acessar o painel administrativo do Django (/admin).

🧭 7. Listar todos os comandos disponíveis
python manage.py help


📘 Exibe uma lista completa de comandos disponíveis no Django.

🧪 8. Executar testes
python manage.py test


🧫 Roda os testes automatizados definidos nos arquivos tests.py.

🐚 9. Acessar o shell interativo
python manage.py shell


💬 Abre o shell Python com o ambiente Django carregado (ótimo para testar consultas e scripts).

🌍 10. Coletar arquivos estáticos
python manage.py collectstatic