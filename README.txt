This is a really nice awesome badass incredible readme for a really nice awesome badass incredible project. (lies)





On Linux :
1) Install geoserver
2) Install Postgresql
sudo apt-get install postgresql postgresql-contrib postgis
3) Install pgAdmin 3
sudo apt-get install pgadmin3
4) Install postgis*



CREATE DATABASE

sudo -u postgres createuser gisuser
sudo -u postgres createdb --encoding=UTF8 --owner=gisuser gis

CHANGE PW
sudo -u postgres psql
THEN \password

\q TO QUIT


psql --username=postgres --dbname=admin -c "CREATE EXTENSION postgis;" 
IF NOT OK, MODIFY IN PGADMIN3 USER PEER INTO MD5 (/etc/postgresql/version/mainpg_hba.conf) AND RESTART SERVER WITH sudo service postgresql restart


5) Install sudo apt-get install osm2pgsql
