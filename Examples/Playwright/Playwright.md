
# PlayWright (WIP)

Example of Using Playwright in Python to Control a Web Page in Chromium

Using Pycharm with pytest and playwright installed I can use the command - `Playwright codegen https://tutorialsninja.com/demo/` to open playwright code Inspector and the test website (Chromium is default but can be changed by adding '- b firefox' into your command e.g. `Playwright codegen -b firefox https://tutorialsninja.com/demo/` ).

![Screenshot_1](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Playwright/Capture2.JPG)

The Playwright Code Inspector opens with pre-generated code to launch the browser and waits for your interactions. As you interact with the browser, it records your actions and automatically generates the corresponding test script code.

![Screenshot_2](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Playwright/Capture3.JPG)

* In this example, I'm logging into tutorialsninja.com. The test mirrors the Java example and shows how eay it is for Playwright to create the automated script:

![Screenshot_2](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Playwright/Animation1.gif)

By copying the code from the Playwright Instpctor i can paste into pycharm and run the script as normal to see the test play out.

![Screenshot_3](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Playwright/Animation2.gif)

# Pytest



