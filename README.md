# Heroku buildpack for KrakenD

A buildpack for Heroku for running [KrakenD](https://www.krakend.io/). 

## Using the Heroku Node.js buildpack

    heroku buildpacks:set https://github.com/InterfloraDanmark/heroku-buildpack-krakend

## Configuration
A default `Procfile` will be created automatically if it does not exist with the following content:

    web: krakend run -c krakend.json -p $PORT

Place your `krakend.json` in the root of your project and it will automatically be used.
