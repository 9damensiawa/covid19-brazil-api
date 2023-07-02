
 
# How to Use IAR Embedded Workbench for STM8 1.40.1
 
IAR Embedded Workbench for STM8 is a powerful development toolchain that provides a complete solution for creating, debugging and optimizing applications for STM8 microcontrollers. In this article, we will show you how to use IAR Embedded Workbench for STM8 1.40.1 to develop a simple LED blinking project for an STM8S103F3 device.
 
**Download Zip ››››› [https://shurll.com/2uypF5](https://shurll.com/2uypF5)**


 
## Step 1: Install IAR Embedded Workbench for STM8 1.40.1
 
To install IAR Embedded Workbench for STM8 1.40.1, you need to download the installer from the [official website](https://www.iar.com/products/architectures/st/iar-embedded-workbench-for-stm8/) and follow the instructions. You can choose either a 14-days trial version or a size-limited version[^2^]. The installation process is straightforward and should not take more than a few minutes.
 
## Step 2: Create a New Project
 
After installing IAR Embedded Workbench for STM8 1.40.1, you can launch it from the Start menu or the desktop shortcut. To create a new project, go to File > New > Workspace and select a folder to save your workspace. Then, go to Project > Create New Project and select C Executable Project as the project type. You can name your project as you like and click OK.
 
The next step is to select the device you are using. In this case, we will use an STM8S103F3 device, which is part of the STM8S series of devices[^3^]. To select the device, go to Project > Options > General Options > Target and click on Device Database. Then, type STM8S103F3 in the search box and select it from the list. Click OK to confirm your selection.
 
## Step 3: Write the Code
 
Now that you have created your project and selected your device, you can write the code for your application. In this example, we will write a simple code that toggles an LED connected to pin PD0 of the STM8S103F3 device every second. To write the code, go to File > New > Source File and name it main.c. Then, copy and paste the following code into the editor:
 `#include 

#define LED_PIN PD_ODR_ODR0 //define LED pin as PD0

void delay_ms(unsigned int ms) //define a function to generate delay in milliseconds

  unsigned int i,j;
  for(i=0;i` 
The code includes the header file iostm8s103f3.h, which contains the definitions of registers and bits for the STM8S103F3 device. It also defines a macro LED\_PIN as PD\_ODR\_ODR0, which is the output register bit for pin PD0. The function delay\_ms generates a delay in milliseconds by using nested loops. The main function sets the clock frequency to 16 MHz by writing 0x00 to the CLK\_CKDIVR register, sets PD0 as output by writing 1 to PD\_DDR\_DDR0 bit, sets PD0 as push-pull by writing 1 to PD\_CR1\_C10 bit, and then enters an infinite loop that toggles PD0 every second by using bitwise complement operator (~) on LED\_PIN.
 
## Step 4: Build and Debug the Project
 
After writing the code, you
 8cf37b1e13
 
