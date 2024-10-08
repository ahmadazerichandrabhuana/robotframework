# Test Automation using Robot Framework

This is a simple sample for Test Automation using Robot Framework.

> [!NOTE]  
> This repository uses Browser Library, not Selenium (which might be more popular out there). Documentation can be found [here](https://robotframework-browser.org/).

## Requirements

1. Install [VS Code](https://code.visualstudio.com/) or any Code Editor you're comfort with.
2. Install [Python 3](https://www.python.org/).
3. Make sure 'pip' also installed together with Python 3. If it is not automatically installed, refer to [Python Crash Course](https://ehmatthes.github.io/pcc/chapter_12/installing_pip.html).
4. Update Python to your PATH file. Refer [here](https://realpython.com/add-python-to-path/), this website covered configuration for Windows, Linux, and MacOS.
5. Install [RobotFramework](https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#installing-using-pip).
6. Download and open this code repository on your local system and run these 2 commands :
   ```
   pip install -r requirements.txt
   rfbrowser init
   ```

## Run Tests
* Run all tests : 
   ```
   robot tests
   ```

* Run specific test : 
   ```
   robot tests/{test file name using extention ".robot"}
   sample :
   robot tests/001.robot
   robot tests/002.robot
   robot tests/LoginPageTest.robot
   ```

## Open Test Report

    open report.html

## Open Test Log

    open log.html

## Repository Explanation

This sample Test Automation consists of 3 main folders : 

* config
   ```
   Contains basic configuration of Variables, Settings, and Keyword wich will be used globally on this whole project
   ```
* resources
   ```
   Consists of 3 more folders :
   > helpers  : contains any action which might be used globally on any pages
   > locators : contains web element for each specific web pages
   > pages    : contains actions which will be performed on each specific web pages
   ```
* tests
   ```
   Contains test cases
   ```

Apart from these 3 folders, this sample also using 'env.yaml' file which can be used to store configuration-specific data. On this sample, URL for test is stored there :
   ```
   SauceDemo_URL: https://www.saucedemo.com/
   ```
