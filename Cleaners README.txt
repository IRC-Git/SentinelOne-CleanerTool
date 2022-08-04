Run the Cleaning utility:

Option 1: When 'Self-Protection' is ON and Windows is in Normal mode:
	Open CMD 'as Administrator'
	Run:
	cd C:\SentinelCleaner_<version>.exe -t "Site token for diagnostics" -k "PASS PHRASE FROM STEP TWO"

Option 2: 2When 'Self-Protection' is OFF or the machine is in Safe mode:
	Open CMD 'as Administrator'
	Run: 
	cd C:\SentinelCleaner_<version>.exe -t "Site token for diagnostics"

Follow the guidelines on the CMD window

To make sure that the cleaner was executed successfully, please run the following:

	From CMD: echo %errorlevel%
	From Powershell: $LastExitCode

If the error code is different than 0 (zero - successful execution), please make sure to send it over to Support
Save the CMD history (as it might be needed for further analysis)

Reboot the machine
 
Note: If no Diagnostics are needed please use:
-d 0

Sets if diagnostic information is collected. The default is 1 (enabled) and does not have to be added to the command. 
To run the Cleaner tool without collecting diagnostic information, set d to 0.