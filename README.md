# Custom ArcGIS Online Dashboard Table Formatting with Arcade



This Arcade script is an example in how I formatted my Dashboard's table according to a project's submittal status.
To use, change parameters as needed and paste into advanced formatting when setting up your Dashboard.



This script does the below items:
  - Assigns colors of table rows according to submittal status type
  - Adds a time dependent color for submittals that have been under review for over 30 days
  - Formats a raw date value to be in a MM/DD/YY style
  - Does a date calculation for # of days ago submittal was submitted. (Example: 11/02/2022 (10 days ago))
  - Does a date calculation for # of days taken for feedback from agency (Example: 11/06/2022 (12 days after submittal))
