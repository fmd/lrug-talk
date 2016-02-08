# Rails & Docker for Development: No Mess, No Fuss.

## Installation

* Install the [docker toolbox](https://www.docker.com/products/docker-toolbox).
* Clone this repository: `git clone git@github.com:/fmd/lrug-talk`.
* `cd` into the directory (`cd lrug-talk`) and `docker-compose build`.
* Create our database: `docker-compose run web --rm rake db:create`
* Run the app! `docker-compose up`