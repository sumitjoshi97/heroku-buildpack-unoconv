# Unoconv/LibreOffice buildpack for the heroku-18 stack

Add the `heroku-buildpack-apt` buildpack to your project:
```
heroku buildpacks:add --index 1 https://github.com/heroku/heroku-buildpack-apt.git
```

Add this buildpack to your project:
```
heroku buildpacks:add --index 2 https://github.com/josduj/heroku-buildpack-unoconv.git
```

Create an `Aptfile` file in your project root with the following content only:
```
unoconv
```

Redeploy your project after committing the above file.
