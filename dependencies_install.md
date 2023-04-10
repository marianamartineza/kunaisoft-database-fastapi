<!-- tutorial para crar API Rest con FastAPI desde 0 -->
https://cosasdedevs.com/fastapi/

# Parte 1
python -m venv env
.\env\Scripts\activate
pip install fastapi uvicorn
uvicorn main:app --reload

# parte 2
<!-- crear la base de datos postgres  -->
CREATE DATABASE to_do_list WITH OWNER = <your-database-user> ENCODING = 'UTF8' CONNECTION LIMIT = -1;

<!-- agregar el .env -->
# Database connection
DB_NAME=to_do_list
DB_USER=my-user
DB_PASS=my-pass
DB_HOST=localhost
DB_PORT=5432

pip install python-dotenv
pip install psycopg2
pip install peewee

<!-- generar las tablas -->
from app.v1.scripts.create_tables import create_tables
create_tables()

# parte 3
pip install "pydantic[email]"
pip install "passlib[bcrypt]"