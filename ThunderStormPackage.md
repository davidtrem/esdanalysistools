Note: ThunderStorm is under active development, the following documentation
might be incomplete and possibly incorrect regarding the latest ThunderStorm version.
We will do our best to keep it in sync with the most recent code version.

# Structure of thunderstorm python package #

thunderstorm python package actually group 3 sub-packages:
  * thunder
  * lightning
  * istormlib

## Data manipulation : thunderstorm.thunder ##
thunderstorm.thunder packages group several python modules which constitute
the core of ESD-data handling and manipulation.

The **importers subpackage** group the modules to import data from several testers

## Data ploting : thunderstorm.lightning ##
thunderstorm.lightning package group python modules useful to plot ESD-data.

## Interactive console : thunderstorm.istormlib ##
thunderstorm.istormlib package relates to Istorm which
is a lightweight shell around Thunderstorm library dedicated to simple to very
advanced data manipulation.