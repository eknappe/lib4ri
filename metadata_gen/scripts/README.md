#README for metadata_generation script
##Created by E. Knapppe

This metadata generation script was tailored for uploading data to DataLakes (https://www.datalakes-eawag.ch/?home), but it follows a general format that can be used for other projects. 

The metadata schema is DataCite, which is the new recommendation for all ETH Domain data repositories. More info on DataCite here (https://datacite-metadata-schema.readthedocs.io/en/4.6/properties/description/)

DataCite is typically in JSON format, and this script collects all the necessary metadata from the user via prompting, then converts it into the DataCite JSON formatting. Knowledge of python is not necessary for this script. 

##Prior to use

The script will prompt the user for the information. For certain things, like ORCID ID and ROR IDs, the script will take the prompted information and suggest an option. The user has the option to correct or change items throughout the process.

	Creator = Primary author (first and last name)
	Affiliation = Primary author's current affiliation
	ORCID ID 
	Title = title of the dataset
	Description = abstract explaining the dataset (unlimited characters)
	Publication Year = year the data is being published
	Resource Type = typically 'dataset'
	
	Co-authors
		First and last name
		ORCID ID (will prompt based on first and last name)
		Affiliation (will prompt based on first and last name)
	
	Location of data collection
		Latitude (decimal degrees)
		Longitude (decimal degrees)
		Name of lake

	Time period of data collection
		Start date
		Start time (if applicable)
		End data
		End time (if applicable)
	
	Data license to use (recommend CCBY 4.0)
	DOI = doi of data if published in another repository (if applicable)
	Version = if applicable
	
	Keywords = list of comma separated keywords for ease of searching data (e.g. measurementtype,lakename, etc.)
	

##Use

The script is meant to be run, and then it will prompt the user with the information it needs. Prior Python knowledge is not needed. 




