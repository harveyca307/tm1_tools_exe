TM1ModelDoc.exe:
	This application will output files depending on passed arguments to document assets in TM1 model:
	
	Usage:
		TM1ModelDoc.exe servername <arguments>
	Arguments:
		-m:	Output Excel file of everything in model
		-c:	Output Cubes and associated Dimensions to CSV
		-v:	Output Cubes and associated Public views to CSV
		-t:	Output Cube stats to CSV
		-d:	Output Dimensions to CSV
		-i:	Output Dimensions and associated Hierarchies to CSV
		-a:	Output Dimensions and associates Attributes to CSV
		-s:	Output Dimensions and associated Subsets to CSV
		-o:	Output unused Dimensions to CSV
		-p:	Output TI Processes to CSV
		-r:	Output Chores to CSV
		-e:	Output }ClientGroups to CSV
		-n:	Output }DimensionSecurity to CSV
		-b:	Output }CubeSecurity to CSV
		-f:	Output }ApplicationSecurity to CSV
		-k:	Output }ProcessSecurity to CSV
		-l:	Output }ChoreSecurity to CSV
		-u:	Output unused Security Groups to CSV

tm1_backup.exe:
	This application will use 7-zip (http://7-zip.org) on the server to create a compressed backup of the TM1 database
	
	Usage:
		tm1_backup.exe -s <database directory> -d <location for backup file> -v <server name> options...
	
	Arguments:
		-s <source>:		Source directory
		-d <destination>:	Destination directory
		-s <server name>:	TM1 Instance Name
		-c <files to keep>:	Number of backup files to keep
		-f:					If used, FEEDER files will be backed up

tm1_logs.exe:
	This application will help maintain Logging directory.  Any file that is deleted will be notated in "Log_Deletions.txt" file with date of removal.
	
	Usage:
		tm1_logs.exe -s <logging directory path> -d <number of days logs to retain>
		
	Arguments:
		-s <path>:	Logging Directory Path
		-d <days>:	Retention period for TM1 Logs