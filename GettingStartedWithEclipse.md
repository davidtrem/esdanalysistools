# Getting Started With Eclipse #
## Install Mercurial Eclipse ##
In Eclipse: Help -> Install New Software -> Install dialog

Add the following software site:
  * Name: `Mercurial Eclipse`
  * Location: `http://cbes.javaforge.com/update`
  * -> OK
  * Select this repository from the pull down menu.
  * Select package `MercurialEclipse`
  * You will get a message stating that you are installing unsigned content.
  * Press OK and accept the exception by ticking the item in the list above!
  * OK
  * Eclipse proposes to restart, OK. Done!

## Add Mercurial Repository from Google Code ##
  * File -> Import ...
  * Mercurial -> Clone Existing Mercurial Repository
  * Next >
  * Browse with your webbrowser to your Google Code clone page that you want to import and select "Checkout"
  * Copy the https address from the mercurial command line access: `hg clone https://yourrepository.googlecode.com/hg/ yourrepository`
  * Paste it into the URL field and leave the rest open (Optionally you may want to change the directory name to a more readable format). Next >
  * You may have to press Next > another time
  * Select working directory revision. Next >
  * Finish!

## Problems internet connection in Eclipse ##
In case you have issues with importing a mercurial repository, you may have to specifiy manually your proxy host:
  * Help -> Preferences
  * In Preferences dialog: General -> Network Connections
  * Set Active provider to "Manual"
  * Specify the proxy for at least HTTP and HTTPS (Host name, port, optionally user credentials)
  * OK

## Run problems ##
This section presents some common issues that occur.
### Import Error ###
**Problem:** the following error occurs when you want to start the Satellite GUI (CTRL+F11):
```
Traceback (most recent call last):
  File "<<path>>\satellite.py", line 38, in <module>
    from thunderstorm.thunder.importers.tools import plug_dict
ImportError: No module named thunderstorm.thunder.importers.tools
```

**Prequisites:**
  * Populated (mercurial) project for Satellite
  * Populated (mercurial) project for Thunderstorm

**Solution:**
With Thunderstorm project:
  * Right click on the project in Pydev Package Explorer
  * Pydev > Set as Pydev Project
  * Right click again
  * StartExplorer > Copy resource path
With Satellite project:
  * Open file satellite.py
  * Right click on project file > Properties
  * PyDev - PYTHONPATH > External Libraries > Add source folder
  * Paste path in to the field > OK

### py2app or py2exe related issues ###
If you want to start Satellite, but get a message that looks like:
```
ImportError: No module named py2app
ERROR: Module: setup-py2app could not be imported.
```

Try from Eclipse menu:
  * Run > Run As > Python Run

Another solution may be to close and remove `setup-py2app.py` and `setup-py2exe.py`