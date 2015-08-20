Towds is a geolocation based marketplace, similar to an online fleamarket.

Requirement:

	* GEOS - http://trac.osgeo.org/geos/
	* proj - http://anonscm.debian.org/cgit/pkg-grass/proj.git


If using a database besides SQLite3 install the plugins listed here - https://docs.djangoproject.com/en/dev/ref/contrib/gis/install/geolibs/

Run 'pip install -r requirements.txt' to install required python extensions 

Files and directory:

	ads/			Listings live here
	core/			Base application
	profile/		User profile info lives here
	requirements		Django python required extensions
	towds/			Towds configurations
	towds_api/		API REST backend
	README			This file


How to start:

    $ copy towds/settings_copyme.py to towds/settings.py and enter db info and django secretkey
    $ python manage.py syncdb
    $ python manage.py runserver

Finally, go to http://127.0.0.1:8000/ in a browser

