# Messing around with NBA data using flask and d3
#forking https://github.com/adilmoujahid/DonorsChoose_Visualization

## Getting started

The dependencies for the project can be installed using

    $ pip install -r requirements.txt

Use ``Vagrant`` to start a machine with a MongoDB instance running

    $ vagrant up

Initialize the database you need to download the data

    $ wget http://s3.amazonaws.com/open_data/opendata_projects000.gz && unzip opendata_projects000.gz

and import it

    $ mongoimport -d donorschoose -c projects --type csv --file /vagrant/opendata_projects.csv -headerline
