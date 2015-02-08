# Wunderpal

## chrome extension for wunderkraut project annotation

Learning project for angularJS

## Steps to rebuild

GIT-Tag v0.0.1

1. start a chrome extension project with a manifest.json
Easy start with a web scaffolding tool:
http://extensionizr.com/

2. enable extension in chrome by activating the developer mode here:
chrome://extensions/
and load unpacked extension from disk

GIT-Tag v0.0.2

3. More info about building a chrome extension can be found here:
http://code.tutsplus.com/tutorials/developing-google-chrome-extensions--net-33076

4. Create a (backup) data store with an api that can be used by angularJS. We use Google spreadsheets and the Google script api. [http://www.google.com/script/start/](http://www.google.com/script/start/)
The script is saved in this repo /js/Code.gs for reference in its early state
The spreadsheet that acts as a data store/source is
[drupal module choices datastore](https://docs.google.com/a/wunderkraut.com/spreadsheets/d/1ktfyqSrFXYwlYOV4qvesAfZjccfrex_ZIxEqY67HRd0/edit?usp=sharing)
At the moment we still have to figure out if we can integrate this as a service or if we have to use the public spreadsheets api

5. Set up the angular project folder structure and build the app with npm/bower
	* initialize a bower package file by running `bower init` in the command line
	* then "install" the dependencies by running `bower install angular --save`
	* modify manifest file to inject angular and vendor scripts into all drupal pages
	
6. Inject views and the angular app into the page
