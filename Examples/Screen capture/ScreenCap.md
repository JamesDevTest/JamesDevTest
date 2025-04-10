
# Test Script Generator

Below is an example of a VBA script that Grabs a screenshot using ScreenClipping. It takes current cell and uses the cell reference to rename the screen captuer so the image is always associated with the correct step. I uses the cell height and width to resize the image to fit into the cell so you can easily start adding second or third screenshots for each test step in a row while keeping the test script clean and neat.


![Screenshot_1](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Screen%20capture/Animation1.gif)

You can click on the screenshot to enlarge the image back to the original size and back again.

![Screenshot_2](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Screen%20capture/Animation2.gif)

This will load the data we will use to create the test cases. The ID relates to a customer, The Sub EDR relates to the test that will be ran And Descritpion is the discription of the EDR type e.g EDR 2 is a adverse press check review. The Type will indicate the what test step will be needed. If i start the creation process by selecting Scripts from the 'menu' and press on 'Create Scripts'

![Screenshot_3](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Screen%20capture/Animation3.gif)

The Python code iterates throught the Test Data and creates a test script for each ID. 

![Screenshot_4](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Screen%20capture/Animation4.gif)

The scripts will be generated and saved as excel files and stored in the script folder.

![Screenshot_5](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Screen%20capture/Animation5.gif)

The Script template is loaded and populated with date found on external spreadsheets to create the expexted test output code as well as customer details and test steps.

![Screenshot_6](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Screen%20capture/Animation6.gif)



