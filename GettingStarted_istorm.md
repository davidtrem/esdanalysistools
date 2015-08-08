# Introduction #
istorm is a light weight shell around Thunderstorm library.
It gives access to basic functionality of Thunderstorm.


# Install a scientific Python environment #
## On Windows platforms ##
For Windows users, the easiest way is to install
[Python(x,y)](http://www.pythonxy.com/) distribution.
Please follow the instruction on this website.
## On Unix/Linux platform ##
Install
  * Python 2.6,
  * numpy,
  * matplotlib and
  * ipython
using the install tools available for your Unix/Linux distribution.


# Download and unpack Thunderstorm bundle #
You can download the latest source from the Downloads tab
in the upper part of this web page.
Then:
  * Unzip the file
  * Open the created directory
In this folder you will see the istorm.py file


# Run istorm... #
## Windows users ##
To run istorm drag and drop the folder containing your tester data on the istorm.py file (see previous section to locate it).
## Unix/Linux users ##
Open a terminal window and change folder to go to the unziped ThunderStorm directory.<br />
In this folder run istorm:
`python istorm.py`
This command will launch istorm


# ...and start playing! #
Available tester import plugins will be displayed after startup.

Unix/Linux users following this Getting Started will have to
change to their TLP data directory before continuing.<br />
For this, as in a terminal shell _but within istorm_, type:<br />
`cd /My/TLP/Data/folder/path`<br />
Please, replace "/My/TLP/Data/folder/path" by the path where your TLP data folder is located.

Use Load.'tester\_plugin\_name'("datafile") to load a measurement

For example for Oryx tester data
```
exp1 = Load.Oryx("datafilename.tsr", "my own data description")
```
Then you can create a View for your data
```
view1 = View(exp1)
```
You can then plot the classical TLP graph
```
view1.raw_tlp_with_leak()
```
...