# Sector file
## Welcome to the XT Sector File

Thank you for your interest in the XT Sector File. In this GitHub you will have the opportunity to contribute directly to sector file changes, and raise existing issues for the team to look at. 

## How to contribute?

### Raise existing issues with the team
To raise an issue with our sector file team, head to the Issues page and create an issue. The team will then tag it and action it as appropriate.

### Contibute to changes
To contribute to the sector file, first create a fork of the sector file, this will be your version to work on. Make changes as required, then when you're ready to submit the changes, submit a pull request and this will be reviewed by our team. 
You can use the following HQ guidance to help. Alternatively feel free to reach out for assistance in the XT discord. 
https://wiki.ivao.aero/en/home/devops/manuals/SectorFile_Definition

## Sections

### 01-Nav Data
The Nav Data section contains fixes, NDBs, VORs, airways, and airspace. With the exception of airspace, this information is imported from the AIP using IAB. 

### 02-Airport Data
The Airport Data section contains basic airport information in the airports and rwys files. This is what populates the 'Airports' tab information on Aurora. This information is imported from the AIP using IAB. 

### 03-SID/STAR Data
The SID/STAR data includes all the SID & STAR information in the sectorfile. This information is manually processed using coordinates generally from the AIP or Navigraph (for those with a subscription). 
  1. .sid files: contain the SIDs for aerodromes
  2. .str files: contain the STARs and IAPs for aerodromes

### 04-Airport Mapping
Airport Mapping is the main section of the sector file that users will edit, and this is where we build our ground maps. There are 4 types of files that make up our ground maps. These are as follows:
  1. .apt files: contains line markings including taxiway edge & centrelines, apron edgelines, runway edge lines, stand centrelines (piers), holding points, and building outlines.
  2. .gts files: contains gate information (generally imported from AIP using IAB but sometimes manually tweaked to fit the sector file visually.
  3. .tfl files: contains the colourful side of the ground map, including runways & markings, taxiways, aprons, buildings. Also contains the shading for online airport level ATC (aerodrome & approach level).
  4. .txi files: contains the taxiway labels for the aerodrome. This information is manually processed.

### 05-VFR Routes & Fixes
Contains the VFR routes and fixes. Consists of 2 types of files:
  1. .vfi files: visual fixes
  2. .vrt files: visual routes

### 06-En Route 
Contains miscellaneous files impacting en route including:
  1. .geo files: containing outlines of the black sea coast and caspian sea coast
  2. .tfl files: similar to the tfl files in 04, but contains the shading for online en route level ATC (Radar/Control).
  3. artcc file: contains the en route/FIR boundaries

### 07-MVAs
Contains the mimimum vectoring altitude (MVA) files for aerodromes in XT.

### 08-Special Areas
Contains special area files (danger, restricted & prohibited areas).

### 09-ATC
Contains the ATC file which defines the controlling positions and their frequencies. 
