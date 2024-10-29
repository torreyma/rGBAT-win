# rGBAT-win
This git repo provides R packages that will allow you to use NYC DCP's powerful [Geosupport](https://www.nyc.gov/site/planning/data-maps/open-data/dwn-gde-home.page) geocoding software in R on Windows. For a Linux version, see: https://github.com/torreyma/rGBATl

## Installation
1. Manually download NYC's Geosupport version 24B from Bytes of the Big Apple:
    * Search for "Geosupport Desktop Edition™ - Windows version (64-bit)" on NYC DCP's [BYTES of the BIG APPLE™ Archive](https://www.nyc.gov/site/planning/data-maps/open-data/bytes-archive.page) page.
    * Or try this url for direct download: https://www.nyc.gov/assets/planning/download/zip/data-maps/open-data/gde_20b_x64.zip 
        * (Should work if DCP hasn't changed anything.)
2. Run the Geosupport installer. Note: you need Admin permissions to install.[^1]
3. Clone this repo to your computer.
4. In R, open ```install_rGBAT20B.R```. 
    * Make sure your working directory is the top-level folder of the repo you cloned. 
        * The file rGBAT-temp_packages.zip is included in the repo. Do not unzip it, the R code will do that for you.
    * Then run the code in install_rGBAT20B.R
    * This should compile and install the rGBAT package. (This is an R package.)
        * If you get an error about missing ```NYCgeo.h```, you haven't installed Geosupport correctly. Remember, you have to do that first.
    * A directory ```temp_packages``` will be unzipped in your HOME directory. This contains the R package source code, if you want to review it.
        * You can delete the ```temp_packages``` directory after the package installs.
5. Once the package successfully installs, you can load the package and check the help for how to use it, in R:
    * Load the library: ```library(rGBAT)```
    * Look at the help for the package: ```help(package=rGBAT)```
    * See the help for a specific function, something like ```?GBAT.process_freeform_addresses```
    * In the help for the function will be some example code you can run. Run that code in R and see if it works correctly. This is a good test to run before you try geocoding your own addresses.

[^1]: (I do not have Admin permissions on my only Windows box, so I haven't actually tested any of this! If you do try this, let me know how it goes.)

## License and credits
* The original package, rGBAT, was written by Gretchen Culp (https://github.com/gmculp), initially exclusively for use on DOHMH's RHEL R server. (rGBAT-win simply extends its use to generalized Windows for the public.)
* This package is released under an MIT license (see LICENSE file).
* Geosupport Desktop Edition™ copyrighted by the New York City Department of City Planning. This product is freely available to the public with no limitations. 



