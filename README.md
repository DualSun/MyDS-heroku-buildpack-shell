# MyDS-heroku-buildpack-shell
Heroku buildpack for shell only applications

## Usage
This buildpack allows you to create an app with an executable shell script only.
It detects the presence of the following files at the base of your project :
- a mandatory `app.sh` that can be run manually with the `heroku run bash app.sh` command
- an optional `compile.sh` that can be run on the build phase

## NB
The `app.sh` is not run on each release, you are free to cutomize that or setup a scheduler
