# DiskSpaceRDL
This is a bash script to include computer disk space in CODAR RDL file header

Reporting the disk space of the CODAR acquisition computer has been a long held request for HFRnet site diagnostics. The bash script NewRadial is provided by CODAR as a hook to run after creation of a Radial file.
The script uses the FreeBSD utility "df" to provide disk usage, and then, using "awk", the information is formatted and insertted into the Radial file.
The script should run without any issues on a standard Mac OSX install, just be sure that the /tmp directory exists.

To install, place the NewRadial file into the /Codar/Seasonde/Users/Scripts directory. You should see output in the AnalyzeSpectra window after a Radial is created that reflects the disk information. You should also see the output in the first few lines of the header. 
