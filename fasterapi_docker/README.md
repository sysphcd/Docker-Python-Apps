
# Python app using FastAPI 
python3 -m venv venv

. venv/bin/activate

pip install fastapi

pip install uvicorn

create main.py

paste in the fastapi example from https://fastapi.tiangolo.com/



teminal -> pip freeze > requirements.txt
docker build -t python-fastapi
docker build -t python-fastapi .

in main.py :
if __name__=='__main__':
    uvicorn.run(app, port=8000, host="0.0.0.0")
    
docker build -t python-fastapi    
docker run -p 8000:8000 python-fastapi 
