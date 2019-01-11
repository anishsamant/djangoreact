1. Inside `backend` Directory
   1.1 `$ virtualenv env` //create a virtual environment

   1.2 `$ .\env\Scripts\activate` //activate the env

   1.3 `$ pip install django`

   1.4 `$ pip install djangorestframework`

   1.5 `$ django-admin startproject djreact`

   1.6 `$ pip install django-cors-headers`

   1.7 `$ pip install django-rest-auth`

   1.8 `$ pip install django-allauth`

2. Inside `backend/src` Directory
   2.1 `$ python manage.py makemigrations`

   2.2 `$ python manage.py migrate`

   2.3 `$ python manage.py createsuperuser`

   2.4 `$ python manage.py startapp articles` //create articles app

   2.5 `$ python manage.py runserver` //to run the server(127.0.0.1:8000)

3. Inside `frontend` Directory
   3.1 `$ create-react-app gui` //creates a react application

4. Inside `frontend/gui` Directory
   4.1 `$ npm start` //to run the server(localhost:3000)

   4.2 `$ npm install antd --save` //ant design library

   4.3. `$ npm insatll axios --save` //library used to get the data off the server

   4.4. `$ npm install --save react-router-dom` //used for redirecting and navigation between pages

   4.5. `$ npm install --save react-redux`

   4.6. `$ npm install --save redux redux-thunk` //middleware
