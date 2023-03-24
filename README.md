![](https://res.cloudinary.com/deepjyoti30/image/fetch/f_auto,q_50,w_2048/https://raw.githubusercontent.com/deepjyoti30/blog-static-content/master/content/Mongo_plus_Heroku.jpg)

## Heroku buildpack: Mongo Database Tools

This is a heroku buildpack that installs all the mongo database tools commands for Ubuntu 22.04.

### The following commands are installed:

✅ bsondump

✅ mongodump

✅ mongoexport

✅ mongofiles

✅ mongoimport

✅ mongorestore

✅ mongostat

✅ mongotop

## Usage

Example usage:

    # create new app, starting with this buildpack
    heroku create --buildpack https://github.com/Daltron/heroku-buildpack-mongo-database-tools.git

    # add buildpack to an existing app
    heroku buildpacks:set https://github.com/Daltron/heroku-buildpack-mongo-database-tools.git -a <app-name>

    # pushing to heroku will then create a new release using this buildpack
    git push heroku master
    
#### Looking for a way to backup your mongo databases automatically on Heroku to S3?
Check out [Safety Net Heroku](https://github.com/Daltron/safety_net_heroku)