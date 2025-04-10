
# Test Script Generator

Below is an example of a python script that creates Test scripts for each set of data stored on a csv file. The test script template is opened and populated with date from the test data and also collects customer details form a customer database stored on excel and details of expected outcome codes stored on seprate excel sheet. Test steps are derived based on the test type from the test data.


![Screenshot_1](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Capture.JPG)

Tkinker is used to create the interface. From the file menu iv selected Load Test Data.

![Screenshot_2](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Capture2.JPG)

This will load the data we will use to create the test cases. The ID relates to a customer, The Sub EDR relates to the test that will be ran And Descritpion is the discription of the EDR type e.g EDR 2 is a adverse press check review. The Type will indicate the what test step will be needed. If i start the creation process by selecting Scripts from the 'menu' and press on 'Create Scripts'

![Screenshot_3](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Animation4.gif)

The Python code iterates throught the Test Data and creates a test script for each ID. 

![Screenshot_4](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Capture5.JPG)

The scripts will be generated and saved as excel files and stored in the script folder.

![Screenshot_5](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Animation3.gif)

The Script template is loaded and populated with date found on external spreadsheets to create the expexted test output code as well as customer details and test steps.

![Screenshot_6](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Animation.gif)
![Screenshot_7](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Animation2.gif)

When the script is populated it will look like this.
![Screenshot_7](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Animation5.gif)
