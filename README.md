# Real Time Operating System - RTOS
Building my own Real Time Operating system using ```STM32F411 MCU``` which is based on ```ARM-Cortex-M4``` architecture. The development board which I'm using is ```Nucleo-F411RE```.[Details of Nucleo-F411RE](https://www.digikey.in/en/maker/blogs/st-nucleo-a-powerful-low-cost-alternative-to-the-arduino)

## Documments Required

The following doccuments will help in buiding our own RTOS :
1. [STM32F411 MCU Reference Manual](https://www.st.com/resource/en/reference_manual/rm0383-stm32f411xce-advanced-armbased-32bit-mcus-stmicroelectronics.pdf) - This will contain information about STM32F411 micro controller unit registers and what they are used for
2. [ARM-Cortex-M4 User Guide](https://developer.arm.com/documentation/dui0553/a/) This consist information about Cystic Timer and features of arm cortex m4
3. [STM32f411 DataSheet](https://www.st.com/resource/en/datasheet/stm32f411re.pdf) - This will contain all the connection details of the board
4. [Nucleo-F411RE User Manual](https://www.st.com/resource/en/user_manual/um1724-stm32-nucleo64-boards-mb1136-stmicroelectronics.pdf) Conists the information of our development board

## Setting up the Project
### Installing the IDE

I have used STM32Cube IDE for my development but there are other options as well you can use them also. For quick comparision you can visit these blogs : 
1. [What are the preferred Integrated Development Environments (IDEs) for STM32 microcontrollers?](https://community.st.com/s/article/what-are-the-preferred-ides-for-stm32-microcontrollers) 
2. [STM32CubeIDE](https://blog.st.com/stm32cubeide-free-ide/)
3. [Keil vs STM ide](https://community.st.com/s/question/0D53W00000U7PcHSAV/keil-vs-stm-ide)

STM32CubeIDE can be downloaded from [here](https://www.st.com/en/development-tools/stm32cubeide.html)

### Downloading the required library
Each register has it's own 32 bit hexadecimal value and it will be very difficult for me to remember or lookup in user manual every time I need to use them, so instead what I can do is use the name already defined by STM CMSIS library, can be found [here](https://github.com/STMicroelectronics/STM32CubeF4). For now I only need two folders for my project and those are [Folder1](https://github.com/STMicroelectronics/STM32CubeF4/tree/master/Drivers/CMSIS/Include) and [Folder2](https://github.com/STMicroelectronics/STM32CubeF4/tree/master/Drivers/CMSIS/Device/ST/STM32F4xx/Include)
