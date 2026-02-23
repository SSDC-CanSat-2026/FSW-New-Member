# FSW-New-Member
New member project for FSW to learn about STM32 by having members write a snesor driver in SPI and then using the data to an XBEE radio in USART.

Made by **Sarah Tran** and **Joel Kubinsky**.

## What will you be doing?
You will be learning about understanding an existing Real-Time Operating Systems with the STM32. Afterwards, you will be writing driver code to translate sensor information to something that the STM32 can use. That information is then going to be sent to an XBEE radio to show on a Ground Control Station (which you do not need to code).

We will also be walking you through important code structures that will be important to understand before writing the driver code. If you do not care about it for some reason, you can skip to [here](#writing-driver-code-for-sensors).

### Requirements:
- Understanding of a programming language (ideally C or C++). This project is done in C.
- [STM32CubeIDE](https://www.st.com/en/development-tools/stm32cubeide.html) (use a guest account with your UFL email).

**NOTE**: STM32CubeIDE's website can be a little slow sometimes, try asking your team lead if they have a version downloaded already. If not, try again later.

We are using an **STM32**G491​RCT6 (as of 2025-2026 CanSat) and so requires the STM32CubeIDE to automate a lot of the code! **When asked which version, just go with the newest.**

## Importing an STM32 project
After opening a workspace, it should look something like this:
![STM32 Homescreen](Images/STM32Home.png)
On the top left corner, click "File" -> "Open Projects from File Systems".    

## Writing Driver Code for Sensors
SPI     - Reading ICM42688\
USART   - Writing to XBEEs

## Extra Resources
- Learn more about [SPI](https://youtu.be/MBwtJhO6b0I?si=Nb-yW6-bYA13eYJV) and [USART](https://youtu.be/fkVYkDuB_38?si=hZDJfQHnWz25cNov) from Dr. Schwartz here at UF.
  