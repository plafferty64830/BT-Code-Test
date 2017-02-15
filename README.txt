Owner: Patrick Lafferty

Router Patch Checking System Version 1.0 15/02/2017

DEVELOPERS CONTACT DETAILS
--------------------------

Should there be any questions please do not hesitate to contact me using the details below:

Email Address 	= pat.lafferty@btinternet.com
Contact Number	= 07873773233
Project link	= https://github.com/plafferty64830/BT-Code-Test
-------------------------------------------------------------------------------------------


GENERAL SYSTEM INFORMATION
--------------------------

- This is a Router Patch checking system which addresses the following tasks:

	- Reading a csv file
 	- Output entire contents of csv file to the screen
  	- Using for loops apply the following filters:
  		-- The router has not already been patched
  		-- The current version of the OS is 12 or above
 		-- There are no other routers which share the same IP address
 		-- There are no other routers which share the same hostname
 
 	- Output all routers that satisfy the conditions
	- System exit

---------------------------------------------------------------------------------

INSTRUCTIONS FOR RUNNING THE SYSTEM VIA THE WINDOWS COMMAND PROMPT (Windows 10)
-------------------------------------------------------------------------------

1.  Create a folder in the local drive called BTCode
2.  Go to BTWorkspace\RouterPatchCheck\src\codeTest
3.  Copy the Main.java file and paste it into the BTCode folder created in the local drive
4.  Open the Main.java file (from the BTCode folder), delete the "package codeTest;" line and save the file 
5.  Also download or copy a version of the sample.csv file and paste it into the BTCode folder
6.  Open the windows command prompt
7.  Change the current path to the BTCode folder (use the "cd \BTCode" command)
8.  Use the following command to set the path of the jdk bin folder:
	 set path="C:\Program Files (x86)\Java\jdk.8.0_121\bin"
    As the above path is the location of my jdk please navigate to the bin folder of your jdk.
9.  Use the dir command to ensure the Main.java file and sample.csv are in the BTCode folder
10. Type in the following command to produce bytecode conforming to the Java Virtual Machine Specification:
	 javac Main.java
    The above command should create an additional file called Main.class
11. Check that the Main.class exists using dir
12. Finally run the program by typing "java Main"

INSTRUCTIONS FOR RETRIEVING DESIRED OUTPUT AFTER THE RUNS
---------------------------------------------------------

1. To indicate the program running the system will display the following question:
	Please enter the full name of the Comma Seperated
	Value file that you wish to examine?
2. Enter the name of the csv file which should be sample.csv
3. The system will output an unfiltered list of the routers followed by a list of the 
   routers that meet the conditions in the specified format.

