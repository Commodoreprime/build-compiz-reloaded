# build-compiz-reloaded
Scripts for building compiz from source

The scripts in this repo are based on the ones from this article:

`https://ubuntu-mate.community/t/installing-compiz-reloaded/5875`

as well as the original scripts from northfield.ws (`http://blog.northfield.ws/category/compiz/`)

These scripts are known to work for Ubuntu 18.04 and (according to the article) 19.10 .

# Files in tree explanations

* ./build : Internal script that handles the actual building of each component

* ./components.list : File that houses each name for each component

* ./fetch : Internal script that grabs sources from a url (in this case: www.northfield.ws/projects/compiz/releases/)

* ./install : Internal script that moves the files to their proper locations

* ./INSTALL : Script intended to be called by the user to start the fetch, build, install process

* ./prerequisites : Contains all dependencies (fetched with apt-get) for building as well as running

* ./REINSTALL : Script intended to be called by the user to completly reinstall compiz and components

* ./uninstall : Internal script called by ./REINSTALL to remove components

