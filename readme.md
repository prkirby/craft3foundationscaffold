# Craft 3 CMS mixed with Foundation Magic

## Installation

#### Install Craft 3 with composer

    composer create-project craftcms/craft PATH

#### Remove .gitignore from your new craft project
This is so we can pull in the scaffold repo with no merge issues

    rm .gitignore

#### Initialize git in your project

    git init

#### Add this repo as an upstream and pull it in

    git remote add scaffold git@github.com:prkirby/craft3foundationscaffold.git
    git pull scaffold master

>Unfortunately you can't create a composer project in a non-empty directory,
>and you cant clone a repo into a non-empty directory, so it's the best we got.

#### Clean up the .gitignore to include craft bits

Remove all of the lines after:

    ## Initial Craft ignores, remove after adding this scaffolding ##

#### Install packages.

    npm install

#### Edit config.yml to reflect your dev environment

    PROXY: 'yoursite.localhost' # Change this for your local server

#### Love Life.


#### (Optional)
#### Remove scaffolding remote

    git remote remove scaffold


## npm Commands

#### Run default watch task
    npm run start

#### Build out the project
    npm run build

#### Build for production
    npm run production

###### Note: all needed files are put in /web/dist/ by default.
###### You may need to change this in config.yml for production.
###### You may also want to edit the .gitignore file to match it to your project needs.
