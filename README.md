# Udacity-Linux-configuration-project
Taking a baseline installation of a Linux distribution on a virtual machine and preparing it to host a web applications, including installing updates, securing it from a number of attack vectors and installing/configuring web and database servers.
- IP address : 35.156.69.166
- URL : http://ec2-35-156-69-166.eu-central-1.compute.amazonaws.com
- SSH port : 2200
## Steps made 
- Created Lightsail instance with Ubuntu OS
- Made some configurations as : 
.... 1. Update all currently installed package
.... 2. Create new user named grader and give it the permission to sudo
.... 3. Configure UFW to allow only ports ( 80 - 2200 - 123 )
.... 4. Change SSH port from 22 to 2200
- install the needed applications and dependencies as :
.... - pip
.... - apache2
.... - mod_wsgi
.... - flask
.... - sqlalchemy
.... - oauth2client
.... - httplib2
.... - requests
.... - postgresql
- configure psql database to serve the web application
- clone the project repository from [here](https://github.com/KarimTawfik17/Soccer-top-teams)
- Make a run.wsgi file to serve the application over the mod_wsgi.
- configure the virtual host from apache2 default configuration file.
- Update OAuth authorized JavaScript origins to instance dns 
## Resources helped completing this project
- https://github.com/iliketomatoes/linux_server_configuration
- https://discussions.udacity.com/t/target-wsgi-script-cannot-be-loaded-as-python-module/250750/8
- http://uwsgi-docs.readthedocs.io/en/latest/WSGIquickstart.html
- https://discussions.udacity.com/t/operationalerror-sqlite3-operationalerror-unable-to-open-database-file/250007/5
- https://discussions.udacity.com/t/importerror-no-module-named-flask-on-lightsail/397001
