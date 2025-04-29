
# Test Script Generator

Below is an example of a Python script that generates test scripts for each data set stored in a CSV file. It opens a test script template, populates it with data from the CSV, retrieves customer details from an Excel-based customer database, and pulls expected outcome codes from a separate Excel sheet. The test steps are dynamically created based on the test type specified in the input data.


![Screenshot_1](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Capture.JPG)

The interface is built using Tkinter. From the File menu, select Load Test Data to begin.

![Screenshot_2](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Capture2.JPG)

This action loads the data used to generate the test cases. The ID corresponds to a customer, Sub EDR identifies the test to be performed, and Description provides details about the EDR type (e.g., EDR 2 refers to an Adverse Press Check Review). The Type field determines which test steps will be generated. To begin creating the test scripts, select Scripts from the menu and click Create Scripts.

![Screenshot_3](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Animation4.gif)

The Python code iterates through the test data and generates a test script for each ID.

![Screenshot_4](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Capture5.JPG)

The scripts are generated, saved as Excel files, and stored in the designated script folder.

![Screenshot_5](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Animation3.gif)

The script template is loaded and populated with data from external spreadsheets to generate the expected test output codes, customer details, and test steps.

![Screenshot_6](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Animation.gif)
![Screenshot_7](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Animation2.gif)
![Screenshot_8](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Capture9.JPG)

Once the script is populated, it will appear as follows:
![Screenshot_9](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Test%20Generator/Animation5.gif)

