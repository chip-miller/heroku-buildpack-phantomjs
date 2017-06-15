Heroku buildpack: PhantomJS
=======================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) of PhantomJS(http://phantomjs.org).

Usage
-----

Example usage:

```shell
$ heroku create --stack cedar --buildpack https://github.com/ga-wolf/heroku-buildpack-phantomjs.git

# or if your app is already created:
$ heroku buildpacks:add https://github.com/ga-wolf/heroku-buildpack-phantomjs

$ git push heroku master
```
