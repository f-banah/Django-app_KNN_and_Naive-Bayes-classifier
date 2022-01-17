# Django application
-Architected & built a web application to get project owners in contact with
candidates.
This app contains :
* a recommendation engine with user collaborative filtering based on the algorithm K nearest neighbors (KNN).
* an AI chatbot (conversational robot) based on the Naive Bayes classifier.
* A real time chat.

# Tools:
- Python (Pandas, NumPy, SciPy, Pillow, Requests,Chatterbot and others) 
- UML
- PostgreSQL
- HTML/CSS/JS
- Django.


# Steps
#create a django project named djangoApp and install requirements.txt
cd djangoApp
python -m venv venv
venv\Scripts\activate
pip install --upgrade pip
pip install -r requirements.txt
django-admin startproject project
cd project
python manage.py startapp main

#database : (the used SGBD is postgresql "Pgadmin4" . the details of the database "name, port, password .." exists in the file settings. In this project , the database name is: DBMifactory)
cd djangoApp
cd project
python manage.py makemigrations main
python manage.py migrate

#add superuser (to add the superuser , you should make first migrations to the database , models and the file storage.py)
cd djangoApp
cd project
python manage.py createsuperuser

#run the server (you should add all the files to run perfectly the app)
cd djangoApp
cd project
python manage.py runserver

