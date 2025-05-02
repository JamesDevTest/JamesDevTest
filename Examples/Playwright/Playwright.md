
# PlayWright Codegen (WIP)

Example of Using Playwright in Python to Control a Web Page in Chromium

Using Pycharm with pytest and playwright installed I can use the command - `Playwright codegen https://tutorialsninja.com/demo/` to open playwright code Inspector and the test website (Chromium is default but can be changed by adding '- b firefox' into your command e.g. `Playwright codegen -b firefox https://tutorialsninja.com/demo/` ).

![Screenshot_1](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Playwright/Capture2.JPG)

The Playwright Code Inspector opens with pre-generated code to launch the browser and waits for your interactions. As you interact with the browser, it records your actions and automatically generates the corresponding test script code.

![Screenshot_2](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Playwright/Capture3.JPG)

* In this example, I'm logging into tutorialsninja.com. The test mirrors the Java example and shows how eay it is for Playwright to create the automated script:

![Screenshot_3](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Playwright/Animation1.gif)

By copying the code from the Playwright Instpctor i can paste into pycharm and run the script as normal to see the test play out.

![Screenshot_4](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Playwright/Animation2.gif)

# Trace Recorder/Viewer

Playwright Trace Viewer is a GUI tool that helps you explore recorded Playwright traces after the script has run. Adding the code to my python script just before opening the browser page will start the trace recording

    browser = playwright.chromium.launch(headless=False, slow_mo=3000)
    context = browser.new_context()
    
    # Start tracing before creating / navigating a page.
    context.tracing.start(screenshots=True, snapshots=True, sources=True)
    
    page = context.new_page()
    page.goto("https://tutorialsninja.com/demo/")
    ......
    ...

    ...
    .....
    # Stop tracing and export it into a zip archive.
    context.tracing.stop(path="trace.zip")
    
And to stop the recording i use the above line after all steps have ran.

After running you python test a file called "trace.zip" will be saved in same folder as the python test script. To open this zip file you need to use playwrights trace viewer. You can open the trace from the Terminal : `playwright show-trace playwright\trace.zip` I will look somthing like the below.

![Screenshot_5](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Playwright/Capture4.JPG)

You can see that screenshots get recorded in order of events that occured. These can be selected to view.

![Screenshot_6](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Playwright/Animation3.gif)

Each step records before and after screenshots. So as my email address is added you can view both images of the login page as the email is added

![Screenshot_7](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Playwright/Animation4.gif)

And on Assertions when you have an expected result like the selected item page is displayed and contains specific text on the webpage you can see the expected Return Value within the Call tab.

![Screenshot_8](https://github.com/JamesDevTest/JamesDevTest/blob/main/Examples/Playwright/Capture5.JPG)


# Pytest



