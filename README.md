#### start django   
    virtualenv venv        
    source venv/bin/activate          
    cd mysite          
    python manage.py runserver        

#### setup env  
    pip install virtualenv     
    virtualenv venv     
    source venv/bin/activate   
    pip install Django        
    pip freeze > requirements.txt    
    pip install -r requirements.txt      

#### setup new project
    django-admin startproject django_postgres     
    cd django_postgres    

#### setup superuser
    python manage.py createsuperuser        
  
#### setup database
    //open local postgress database
    pip install psycopg2

    //setup database       
    python manage.py migrate           
    python manage.py runserver     

#### setting for local postgres
    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.postgresql',
            'NAME': 'mydb',
            'USER': 'postgres',
            'PASSWORD': 'Po4820806',
            'HOST': '127.0.0.1',
            'PORT': '5432',
        }
    }

#### reference
    [1] [Postgresql Installation and Configuration For Django](https://www.youtube.com/watch?v=l4BZqgwxoH4)
