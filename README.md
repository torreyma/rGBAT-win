# rGBAT-win
* This is a copy of Gretchen Culps' rGBAT package as she sent it to NYCEM in 2020. 
* This version (at least initially) is set up for Windows.


## files and folders
* initial install/
	* Contains original install zip file and script from GC.
	* Change into this directory and run:
	* install.rGBAT20B.R
		* This is the install R script from GC. 
		* To install in R:
			* Please save the attached ZIP file someplace on your desktop.  Do NOT unzip it. The script will do that.
			* Open this file in a text editor (like the one in RStudio or Notepad++). Locate the line of code where the path of the ZIP file is specified and change it to where you saved the ZIP file on your local machine (Line 19 maybe?). 
			* Execute the code in this file in R.
			* Close your R session. 
			* Open a fresh R session.
			* Enter the following lines of code in the console to load the package and launch its help documents:
				```library(rGBAT)```
				```help(package = "rGBAT")```
			* Try some of the code samples in the help files
		* (See emails from GC 2023-05-05 12:00 for more details.)
	* NYCEM_packages.zip
		* This is the zip file that contains the rGBAT R packages. 
		* Note that according to the instructions this is used _as_ a zipped zip file when you run the install_rGBAT20B.R script.
* rGBAT and rGBAT20B are what unzips from NYCEM_packages.zip
	* they contain data that is too big (100MB+) to commit to github
	* So you have to unzip NYCEM_packages.zip to get them
	* they contain the actual code / R packages



