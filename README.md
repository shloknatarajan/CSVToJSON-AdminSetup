# CSVToJSON-AdminSetup
Converting CSV files for group and steps into JSON/XML for Admin Setup

Hello everyone, my name is Shlok and I am one of the interns on the Healthcare Cloud team. This python file converts 2 separate CSV files, one for the groups and one for the steps, into JSON and XML Files.

This code isn't finalized as it's missing functionality for the helpUrlLabel attribute and doesn't do any of the validations done within the parser (so if you create a file here it isn't certain that the parser will not throw an error upon reading it).

Steps to use this:
1. Create CSV files for groups and steps with all of the necessary attributes saved as columns. Missing attributes will cause an error to be thrown so use the files here in the github as a template.
2. Save the files in the same directory as the Python file
3. Update the hardcoded values in the python file to what's necessary for your work. 'preexisting', 'featureName', 'json_file_name', 'xml_file_name', and 'configXML' are the currently hard-coded values.
4. Run all of the cells
5. Copy outputted JSON and XML file content into your IDE
6. Rebuild to register XML changes

Next Steps:
1. Integrate the helpUrlLabel attribute
2. Create a validation system similar to the parser's to guarantee that the outputted files will not throw errors
3. Make the process for updating the currently hardcoded values smoother
4. Create a process for generating java beans for AdminExecute and preValidation steps. Integrate that process within this system.
5. Group timeToComplete should be the sum of its steps' timeToCompletes
