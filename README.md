# resume_website
a place to build and host a website to display my resume, the work to make the site, and download my resume.


## Django notes 

django websites are single projects that are split into apps
each app handles a self-contained function

for example:
    
    User management: Login/logout, registration, profile settings
    Website functions: upload/download, navigation

django supports the "Model View Controller" pattern [MVC](https://realpython.com/the-model-view-controller-mvc-paradigm-summarized-with-legos/)

1. Request is made to Controller
2. retrieve and organize all of the models 
3. present the final View


**Model** defines the data structure. This is usually a database and is the base layer to an application.
**View** displays some or all of the data to the user with HTML and CSS.
**Controller** handles how the database and the view interact.

with django, it is the controller, and uses a "Model View Template" pattern

What I think know so far:

Django controller needs to know which apps to control
the project view needs to know which template to return to the requester
the project urls handles the routing


Files
__init__.py tells Python to treat the directory as a Python package.
admin.py contains settings for the Django admin pages.
apps.py contains settings for the application configuration.
models.py contains a series of classes that Django’s ORM converts to database tables.
tests.py contains test classes.
views.py contains functions and classes that handle what data is displayed in the HTML templates.

