# apps-website
all codes and content to generate inVisement.com static website

## inVisement Apps Workshop
inVisement workshop is where an app is developed. It is the logical phase.
apps are integrated features, logical level, similar to production environment. Bugs, automated tests, fixes, ... are introduced here. The final product is similar to what users get. Apps pull from applet and basically adds more files and folders and restructure it and integrate but does not edit the original files. It has branches (master, devel, releases, features, hotfixes, ...)

## inVisement app
- indepenedent, big project with continuous development and developer community.
- no serious devOps, just developer, no physical implementation, just logical and code base
- final product is similar to what end user recieves
- many developers participate
- might have feature branches, release branches, and master branch (dah!).
- has logical development structure for files and folders

## inVisement website
contains all code and content and files to generate inVisement.com static website

## Technology
- contents in markdown
- hugo is generator
- hugo-theme is inVisement website theme
- config file stored in hugo-theme folder
- four main folders: content (markdown files), cdn (codes and js and css), data (changing data files), static (for images and logos and website specific files)

## how to use
- install hugo
- clone this repo or download
- cd in to folder
- hugo server --config hugo-theme/config.toml
- browse 127.0.0.1
- generated website is ready to ship for production

## before shipment
change references:
- data ==> data.inVisement.com bucket
- cdn ==> cdn.inVisement.com bucket
move to storage bucket
- .inVisement.com ==> inVisement.com bucket

## how to contribute
email owner
