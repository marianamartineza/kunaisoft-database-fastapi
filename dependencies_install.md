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

# parte 4
<!-- generar token -->
openssl rand -hex 32

<!-- agregar al env -->
# Auth
ACCESS_TOKEN_EXPIRE_MINUTES=1440
SECRET_KEY=e97965045c7df14cb4d5760371e7325104a8f33ad5d00c0a506d6fb09d0047db

pip install "python-jose[cryptography]"
pip install python-multipart

# parte 5 
<!-- crud todo -->

# parte 6 testing 
pip install -U pytest
pip install requests
