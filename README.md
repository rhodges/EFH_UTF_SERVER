# EFH_UTF_SERVER
UTF Grid server config used for the EFH tool

# Installation
* Use [this guide](https://github.com/Ecotrust/PEW-EFH/wiki/Serving-UTF-Grid-Tiles) to install requirements
* Several config files have already been created for your convenience
  * tilestache.cfg - identifies layers and associated mapnik xml
  * tilstache_wsgi.py - configurations for the uWSGI server
  * tilestache.ini - the ini file uWSGI uses, copy it to /etc/uwsgi/apps-available/
    * symlink that to /etc/uwsgi/apps-enables/tilestache.ini
  * nginx-tilestache - the template for the config to give to NGINX to serve both the app and the tiles
* You will need the corresponding shapefiles in the correct locations for this to work
