This wiki explores the open ESD File Format using hdf5

# Stucture #

```
\ESD file        
  \User Data     
     \user name
     \project name                 
     \date           
  \User defined Data                      
     \device name                       
     \device type                       
     \technology                       
     \lot                       
     \wafer                       
     \die
     \package
     \pins
        \zap pin
        \gnd pin
        \extra pin                 
     \comments            
  \Tester Data                       
     \Tester Type                       
     \tester version                       
     \file version
     \pulse width
     \rise time            
  \Calibration input data            
  \Data                       
      \window                      
      \raw TLP data                       
      \waveform data                      
      \leakage data
		\ voltage sweep
		\ current sweep            
  \Calibrated Data
  \Extracted Data
  \user commens
\ESD file 2
...
```