
En celdas individuales en jupyter notebook
poner cada uno de los siguientes códigos para instalar postgresql.

!sudo apt-get -y -qq update

!sudo apt-get -y -qq install postgresql

!sudo service postgresql start


Configuramos la password a postgres del usuario postgres

!sudo -u postgres psql -U postgres -c "ALTER USER postgres PASSWORD 'postgres';"


Creamos la base de datos dvdrental 

!sudo -u postgres psql -U postgres -c 'CREATE DATABASE dvdrental;'

Cargamos la base de datos dvdrental a partir del archivo dvdrental.sql

!sudo -u postgres psql -U postgres dvdrental /content/drive/MyDrive/prueba/dvdrental.sql
