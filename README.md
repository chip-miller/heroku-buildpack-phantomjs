# Heroku buildpack: PhantomJS
=======================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) of PhantomJS(http://phantomjs.org).

## Local Usage

- Install phantomjs
  - e.g. ` brew install phantomjs `
  
## Heroku Usage

- Add the buildpack

```
heroku buildpacks:add https://github.com/jamesnugent00/heroku-buildpack-phantomjs
```

- Change your Heroku paths

```
heroku config:set PATH="/usr/local/bin:/usr/bin:/bin:/app/vendor/bin"
heroku config:set LD_LIBRARY_PATH=/usr/local/lib:/usr/lib:/lib:/app/vendor/phantomjs/lib
```

- Restart your Heroku app
  - e.g. ` heroku restart `
- Create a new deploy
  - e.g. ` git push heroku master `
