# kunaisoft-database-fastapi
implementacion de base de datos sistema kunaisoft 

# iniciar proyecto
python -m venv env

# activar servidor python
./env/Scripts/activate 

# instalar el fastapi y el unicorn
pip install fastapi uvicorn 

# instruccion consola ejecutar un archivo
uvicorn main:api --reload
http://127.0.0.1:8000
