# periodic-worker
A Heroku app that just writes something to app logs

## Setup

```sh
$ git clone
$ heroku create
$ heroku buildpacks:add https://github.com/zunda/heroku-buildpack-sh
$ heroku labs:enable runtime-dyno-metadata
$ git push heroku master
$ heroku ps:scale worker=1
```
