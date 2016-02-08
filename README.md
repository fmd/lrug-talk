# Rails & Docker for Development: No Mess, No Fuss.

## Installation

* Install the [docker toolbox](https://www.docker.com/products/docker-toolbox).
* Clone this repository: `git clone git@github.com:/fmd/lrug-talk`.
* Run `eval $(docker-machine env default)` to bootstrap your Docker environment.
* Run `echo $DOCKER_HOST` and copy the IP to your `/etc/hosts` file. My entry looks like this:

```
192.168.99.100 docker
```

* `cd` into the cloned directory (`cd lrug-talk`) and `docker-compose build`.
* Create our database: `docker-compose run web --rm rake db:create`
* Run the app! `docker-compose up` and visit `docker:3000` in the browser.