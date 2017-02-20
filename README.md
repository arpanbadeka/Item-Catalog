# Item-Catalog
# udacity-catalog #

## Preparations ##

This app uses 

- [Flask](http://flask.pocoo.org)
- [SQLAlchemy](http://www.sqlalchemy.org)

These dependencies must be installed before you can run the app. The easiest way to do so is by using [pip](https://pypi.python.org/pypi/pip). Simply run the following commands:

    pip install Flask
    pip install SQLAlchemy

Next you have to create the categories. To do so run

	python database_setup.py

## Run the app ##

To start the app simply run
	
	python project.py

## Remarks ##
- The app uses nonces to prevent cross-site request forgeries (CSFR) when creating, updating and deleting items.
- The app offers two API endpoints:
	- User JSON: /trainers/JSON
	- User-Pokemon JSON: /trainers/##<int:user_id>##/pokemon/JSON
- The app uses a (slightly modified) **dashboard.css** stylesheet from Bootstrap's [Dashboard sample page](http://getbootstrap.com/examples/dashboard/).
- The app is not optimized for small devices (smartphones etc.).
