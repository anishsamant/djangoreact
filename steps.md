1. Start by creating two seperate folders named `frontend` and `backend`.
2. Create another folder `.vscode` and add the required settings (optional for vscode).

<h2>Backend</h2>
Inside `backend`

3. Create a virtual env and activate it as and when required (1.1 and 1.2).
4. Install `django` (1.3).
5. Install `djangorestframework` (1.4).
   Add `rest_framework` to `INSTALLED_APPS` list present in `settings.py`.
   Add `path('api-auth/', include('rest_framework.urls')),` to `urls.py`.
   Add `REST_FRAMEWORK = {'DEFAULT_PERMISSION_CLASSES': [ 'rest_framework.permissions.DjangoModelPermissionsOrAnonReadOnly' ]}` to `settings.py`
6. Install `django-cors-headers` (1.6).
   Add `corsheaders` to `INSTALLED_APPS` list present in `settings.py`.
   Add `corsheaders.middleware.CorsMiddleware` to `MIDDLEWARE` list present in `settings.py`.
   Add `CORS_ORIGIN_ALLOW_ALL=True` at the bottom of `settings.py`.
7. Install `django-rest-auth` (1.7).
   Add `rest_framework.authtoken` and `rest_auth` to `INSTALLED_APPS` list present in `settings.py`.
   Add `path('rest-auth/', include('rest_auth.urls'))` to `urls.py`.
8. Install `django-allauth` (1.8).
   Add `django.contrib.sites`, `allauth`, `allauth.account`, `rest_auth.registration` to `INSTALLED_APPS` list present in `settings.py`.
   ADD `SITE_ID = 1` in `settings.py`
   Add `path(r'^rest-auth/registration/', include('rest_auth.registration.urls'))` to `urls.py`.
   ADD `ACCOUNT_EMAIL_VERIFICATION = 'none'`, `ACCOUNT_AUTHENTICATION_METHOD = 'username'`, `ACCOUNT_EMAIL_REQUIRED = False` to `settings.py`
9. Create project `djreact`(1.5). Rename the project to `src` (optional).

Inside `backend/src`

7. Make migrations and migrate as and when required (2.1 and 2.2).
8. Create superuser (2.3).
9. Create app `articles` (2.4). Add the app name to `INSTALLED_APPS` list present in `settings.py`.

10. <b>Define the requried content in files created inside `articles` directory.</b>
11. Create `api` folder in `articles` directory to configure the `JSON APIs`.
    <b>Create the required files and define the required content in the corresponding files.</b>

<h2>Frontend</h2>
1. Setup the react app (3.1).
2. Install the `ant design` library (4.2).
3. Install `axios` library (4.3).
4. Install `react-router-dom` (4.4) and `react rekated libraries` library (4.5) (4.6).
5. Create two folders in src `(components and containers)`.
6. Create a `Layout.js` file in containers folder and paste the required `layout` code from ant docs.
7. Create a `Articles.js` file in components folders and paste the required `list` code from ant docs.
8. Create a `ArticleListView.js` file in the containers folder and render the Articles file along with the data to be displayed.
9. Create a `ArticleDetailView.js` file in the containers folder and render the respective article detailed content.
10. Create a `routes.js` file in the `src` directory that manages the component to be rendered at a particular url.
11. Create a `Form.js` file in the containers folder and create a form component for adding and updating the articles.
//----------------------------------------------------------------------------------------------------------------------
//Redux setup
12. Create a `store` folder in src directory. 
    Create `actions` and `reducers` folders in it. 
    Also create a `utility.js` file in it.
13. Create `actionTypes.js` and `auth.js` in `actions` folder.
14. Create `auth.js` in `reducers` folder.
15. Modify the `index.js` and `App.js` files.
16. Modify the `Login.js` and `Signup.js` files in containers folder.
