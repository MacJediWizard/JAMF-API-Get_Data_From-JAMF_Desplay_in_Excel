# JAMF-API-Get_Data_From-JAMF_Desplay_in_Excel
	
### This script runs api calls to get information on Policies, Scripts in Policies, Packages in Policies, Scope in policies, Configuration Profiles, and Scopes in Configuration profiles and save the information in a xlsx document for working with in Excel or similar. 
		
### The Script runs on Python 3 and uses the Libraries "Requests", "Pandas", "openpyxl", and "xlsxwriter". There is a check built in so as long as you have Python3 installed, the other libraries will be installed automatically with pip3.


##	Fields returned in Excel are as follows below:

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


## How to run
	Have python3 on your device. Run the script. Enter the information at the prompts.
	Dependancies will be automatically installed. Enjoy!!!
