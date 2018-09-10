# fio-graphite
Take json output from fio and convert/ship metrics to a graphite instance.

## Environment Variables
* CARBON_HOST
* CARBON_PORT
* METRIC_PREFIX 

## Installation
``pip install git+https://github.com/jordant/fio-graphite.git``

## Example Usage
``fio --name=fio-graphite --rw=readwrite --size=100M --output-format=json | fio-graphite``

![graphite-fio](http://objects.dreamhost.com/public-github/fio-graphite.png)

## TODO
* Stream JSON from fio using --status-interval
* Use graphitesend for shiping 
