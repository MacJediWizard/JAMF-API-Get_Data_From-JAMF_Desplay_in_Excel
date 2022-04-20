# JAMF-API-Get_Data_From-JAMF_Desplay_in_Excel
	
### This script runs api calls to get information on Policies, Scripts in Policies, Packages in Policies, Scope in policies, Configuration Profiles, and Scopes in Configuration profiles and save the information in a xlsx document for working with in Excel or similar. 
		
### The Script runs on Python 3 and uses the Libraries "Requests", "Pandas", "openpyxl", and "xlsxwriter". There is a check built in so as long as you have Python3 installed, the other libraries will be installed automatically with pip3.


##	Fields returned in Excel are as follows below:



###	Computer Info

		if you are usingSmartGroup
		
			Computer SmartGroup ID
			
			Computer SmartGroup Name
			
			Computer Record Type
			
			Computer ID
			
			Computer Name
			
			Computer Serial Number
		
		If you are not usingSmartGroup
		
			Computer Record Type
			
			Computer ID
			
			Computer Name
			
			Computer Serial Number
		
		
		Computer Make
		
		Computer Model
		
		Computer Model Identifier
		
		Computer OS Name
		
		Computer OS Version
		
		Computer OS Build
		
		
		Computer FileVault2 User
		
		Computer Local Account Name
		
		Computer Local Account Real Name
		
		Computer Local Account ID
		
		Computer Local Account is Admin
		
		Computer Local Account in LDAP


	
###	Policy Info

		Policy Record Type
	
		Policy ID
		Policy Name
		Policy Category ID
		Policy Category Name
		
		Policy Target All Computers
		
		Policy Target Computer ID
		Policy Target Computer Name
		
		Policy Target Group ID
		Policy Target Group Name
		Policy Target Group is Smart
		
		Policy Exclusion Computer ID
		Policy Exclusion Computer Name
		
		Policy Exclusion Group id
		Policy Exclusion Group Name
		Policy Exclusion Group is Smart
		
		Policy Package ID
		Policy Package Name
		Policy Package Category Name
		Policy Package Filename
		
		Policy Script ID
		Policy Script Name
		Policy Script Category Name
		Policy Script Filename


	
###	Configuration Profile Info

		Configuration Profile ID
		Configuration Profile Type
		Configuration Profile Name
		
		Configuration Profile Category ID
		Configuration Profile Category Name
		
		Configuration Profile Target Computer ID
		Configuration Profile Target Computer Name
		
		Configuration Profile Target Group ID
		Configuration Profile Target Group Name
		Configuration Profile Target Group is Smart
		
		Configuration Profile Exclusion Computer id
		Configuration Profile Exclusion Computer Name
		
		Configuration Profile Exclusion Group id
		Configuration Profile Exclusion Group Name
		Configuration Profile Exclusion Group is Smart



### Package to Policy lookup

		Provides the following:
		
		Package used or Package Not Used
		in Policies
	
		Which Policy Package is used in. Policies
		or PreStage Policies
		
		Package ID
	
		Package Name
	
		Package File Name
	
		Policy ID if used in a Policy
	
		Policy Name if used in Policy
	
		PreStage Policy ID if used 
		in PreStage Policy
	
		PreStage Policy Name if used 
		in PreStage Policy	


## 	How to run
		Have python3 on your device. Run the script. Enter the information at the prompts.
		Dependancies will be automatically installed. Enjoy!!!
	
		The only requirement is that you have Python3 on the device. All other libraries
		the script will look for them and download if they are not found.
		
		Run from terminal and answer the 3 fields. URL, API Username, API Password.
		You can also send command line args to the script
		For Example : yourScript.py "URL" "API Username" "API Password"
		
		You also get the option to select the path and filename for your xlsx file.
		
		In the Computers section you have the option of running the report with a
		smart group is or on the whole instance.
		
		When looking up local accounts from the computers section, you can do an LDAP
		check to see what accounts are in LDAP. Great for when you use a JIM server.
		
		It will also look up all JIM servers and let you choose the one you want to use.
		
		The script now uses the new bearer token for auth in API calls.
