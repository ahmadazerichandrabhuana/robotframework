# Automation-Test using RobotFramework

This is simple sample for automation-test using RobotFramework.

## Requirements

1. [Pyhton 3](https://www.python.org/)
2. [RobotFramework](https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#installing-using-pip)
⋅⋅⋅or simply run below command

    pip install -r requirements.txt

## Run Tests
* Run all tests : 

    robot -d results tests

* Run specific test : 

    robot -d results tests/{test file using extention .robot}


## Open Test Report

    open results/report.html

## Open Test Log

    open results/log.html
