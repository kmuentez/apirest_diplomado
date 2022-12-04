# Crear primero entorno virtual en terminal VSCODE
  virtualenv venv

# Activar entorno virtual en terminal VSCODE
  .\venv\Scripts\activate.ps1

# Correr requierements.txt
pip install -r .\requirements.txt

# Tener base de datos postgresql y introducir valores de conexión en archivo .env ubicado en la raiz

# Realizar Migraciones

alembic init migrations

# ejecutar
alembic revision --autogenerate -m "crear modelos"
alembic upgrade heads



#  forma de ejecutar fastapi desde la terminal de VSCODE
   uvicorn app:main --reload

# Acceder a la documentación automatica de OPEN API
  http://127.0.0.1:8000/docs
   