heroku-buildpack-pelican
========================

This is a heroku buildpack for Pelican.

```bash
$ heroku config:set BUILDPACK_URL=https://github.com/getpelican/heroku-buildpack-pelican
```

## Configuration

To allow this buildpack to redirect any secondary domains, you can define the
environmental variable `PELICAN_SITEURL`.

```heroku
$ heroku config:set PELICAN_SITEURL=http://getpelican.com
```

Now any requests to `http://pelican.herokuapp.com` or `http://www.getpelican.com` will redirect to the `SITEURL`.

