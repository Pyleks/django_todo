### Useful Django commands

- django-admin startproject name of project .  
> Creates the app it self before starting to code
- python manage.py runserver
> Starts the server
- python manage.py startapp name of app
> Creates the app we will be making
- python manage.py makemigrations --dry-run
> A quick way to see what the migration will do
- python manage.py showmigrations
> This just shows everything that is pre built into a project 
- python manage.py migrate --plan
> This shows what it will do, before doing it.
- python manage.py migrate
> Simply preforms the migration
- python manage.py createsuperuser
> Creates administrator for the website
- python manage.py test
> Runs all the tests scripts
- python manage.py test todo.test_forms
> Runs a specific test Script
- python manage.py test todo.test_forms.TestItemForm
> Runs a specific test script and a specific class within it
- python manage.py test todo.test_forms.TestItemForm.test_fields_are_explicit_in_form_metaclass
> Runs a specific test script and a specific class and a specific test function within it.
- coverage run --source=todo manage.py test
> Check how much of our app we tested
- coverage report 
> Gives us the report
- coverage html
> Gives us a interactive report
- python -m http.server
> Opens a directory to view different directories to access coverage html
- heroku apps:create name of app --region eu


### Initial Django files broken down
#### settings.py
- Container global settings for our project, like showing debug information.
- HTML templates
- What database we connect to.
- When making an app, remember to add the app name here


#### urls.py
- Contains our routing information

#### wsgi.py
- Contains the code the allow our web server to communicate with our application


### Our App files
#### views.py
- Something soon

### Template structure
- templates inside the app folder  
-- todo  
--- html file

> Reason we are putting it inside the todo folder is because it will always return the first one it finds
so by seperating it into a folder that matches the app name, we can ensure we get the right template.

### Migrate
We have to run this to convert out python code sql code.


### Heroku Postgres
To get our database on heroku, we go to our app, then resources, and type postgre,
Choose the Heroku Postgres, and move onto adding it for free.
The configuration for this is revealed in Config Vars