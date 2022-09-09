# Sowa - Django e-learning platform

# About
This is my final project from a SDA course I'm still working on. Sowa is learning platform where we can do tests based on notes.
It has: register/login logic (the profile inheritens from the django.user), editing account with image profile, create notes based on topics(CRUD topic, CRUD note),
blog endpoint. It uses django messages too.

I learned a lot about Django and a bit of JavaScript(+ and - records in Note) because of this project.

# Demo
![Alt text](/sowa_account.png?raw=true "Sowa Account")
![Alt text](/sowa_blog.png?raw=true "Sowa Blog")
![Alt text](/sowa_note.png?raw=true "Sowa Note")
![Alt text](/sowa_test.png?raw=true "Sowa Test")
![Alt text](/sowa_score.png?raw=true "Sowa Score")



## Setup

- ``` git clone https://github.com/kurekhombre/sowa-django-learning-platform.git ```
- Create virtual environment ```python3 -m venv venv``` and activate it
  - Linux/Mac ``` source venv/bin/activate ```
  - Windows ``` venv\Scripts\activate.bat ```
- ``` pip install -r requirements.text ```
- Generate SECRET KEY with 
  - https://djecrety.ir/ or 
  - ``` python manage.py shell ``` 
   ``` >>> from django.core.management.utils import get_random_secret_key``` 
  ``` print(get_random_secret_key) ```
- Create  file '.env' in project folder and paste ``` SECRET_KEY='<your_key>' ```
- ``` python manage.py migrate ```
- ``` python manage.py runserver ```


 # TODO
 - whole INDEX.HTML 
 - improve tests app and correct test view (remove spaghetti code)
 - improve score view
 - overall frontend
 - email link authentication and forgotten password
 - register and login with Google, Apple, Github and so on

