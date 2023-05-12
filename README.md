# GC-rGBAT
* This is a copy of Gretchen Culps' rGBAT package as she sent it to NYCEM in 2020. This version (at least initially) is set up for Windows.


## files and folders
* install.rGBAT20B.R
	* This is the install R script from GC. Instructions:
		* Please save the attached ZIP file someplace on your desktop.  Do NOT unzip it.
		* Open the attached TXT file in a text editor (like the one in RStudio or Notepad++).   Locate the line of code in the attached TXT file where the path of the ZIP file is specified and change it to where you saved the ZIP file on your local machine (I think this is Line 19). 
		* Execute the code in the TXT file in R.  Let me know if you encounter an error.
		* Close your R session. 
		* Open a fresh R session.
		* Enter the following lines of code in the console to load the package and launch its help documents:
			library(rGBAT)
			help(package = "rGBAT")
		* Try some of the code samples in the help files
	* See emails from GC 2023-05-05 12:00 for more details.
* NYCEM_packages.zip
	* This is the zip file that contains the rGBAT R packages. Note that according to the instructions tou use this as a zipped zip file when you run GC's install_rGBAT20B.R script.
* rGBAT and rGBAT20B are what unzips from NYCEM_packages.zip
	* they contain data that is too big (100MB+) to commit to github
	* So you have to unzip NYCEM_packages.zip to get them
	* they contain the actual code / R packages



