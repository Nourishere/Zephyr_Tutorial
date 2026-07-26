 <a href="https://www.zephyrproject.org">
     <p align="center">
       <picture>
         <source media="(prefers-color-scheme: dark)" srcset="notes/images/logo-readme-dark.svg">
         <source media="(prefers-color-scheme: light)" srcset="notes/images/logo-readme-light.svg">
         <img src="doc/_static/images/logo-readme-light.svg">
       </picture>
     </p>
  </a>

# A Zephyr Tutorial
* This repository aims to provide a thorough tutorial on the Zephyr real time operating system (RTOS).
* It is intended for people who are learning about Zephyr, building a project based on Zephyr, or joining Zephyr's developement.
* The repository contains arranged documents in the Markdown format

# Structure
* The repository structure is as follows:
```
examples/
notes/
```
* Under `notes/` you can find arranged tutorial documents with the Markdown format.
* Under `examples/` you can find various Zephyr demo projects.

## Contents
```
notes/
├── 01_Introduction.md
├── 02_ZephyrVsFreeRTOS.md
├── 03_FirstBuild.md
├── 04_WestWorkspaces.md
├── 05_Modules.md
├── 06_Kconfig.md
├── 07_DTBasics.md
├── 08_DTSemantics.md
├── 09_DTPractice.md
├── 10_ADC.md
├── 11_WritingDrivers.md
├── 12_OpenOCD.md
├── 13_Multithreading.md
├── 14_TimersCounterInterrupts.md
├── 15_CustomBoardSupport
├── BONUS_BoardSimulationUsingRenode.md
└── images
```
### Fundamentals
- [Introcuction](notes/01_Introduction.md)
- [Basic Build](notes/03_FirstBuild.md)
  - **Example**: [Hello World](https://github.com/Nourishere/Zephyr_Tutorial/tree/main/examples/hello_world)
- [Kconfig](notes/06_Kconfig.md)
- [Device Tree Basics](notes/07_DTBasics.md)
- [Device Tree Semantics](notes/08_DTSemantics.md)
- [Device Tree Practice](notes/09_DTPractice.md)

### Core Features
- [ADC](notes/10_ADC.md)
  - **Example**: [ADC Demo](https://github.com/Nourishere/Zephyr_Tutorial/tree/main/examples/adc_demo)
- [Modules](notes/05_Modules.md)
  - **Example**: [Custom Module Demo](https://github.com/Nourishere/Zephyr_Tutorial/tree/main/examples/modules/say_hello)
- [Writing Device Drivers](notes/11_WritingDrivers.md)
  - **Example**: [Simple Button Driver](https://github.com/Nourishere/Zephyr_Tutorial/tree/main/examples/modules/button)
- [Multithreading](notes/13_Multithreading.md)
  - **Example 1**: [Threads Demo](https://github.com/Nourishere/Zephyr_Tutorial/tree/main/examples/threads_demo)
  - **Example 2**: [Mutex Demo](https://github.com/Nourishere/Zephyr_Tutorial/tree/main/examples/mutex_demo)
- [Timers, Counters, and Interrupts](notes/14_TimersCountersInterrupts.md)
  - **Example 1**: [Timer Demo](https://github.com/Nourishere/Zephyr_Tutorial/tree/main/examples/timer_demo)
  - **Example 2**: [Counter Demo](https://github.com/Nourishere/Zephyr_Tutorial/tree/main/examples/counter_interrupt_demo)

### Advanced Topics
- [Custom Board Support](notes/15_CustomBoardSupport.md)
  - **Example**: [Custom Support For STM32F4 Discovery Board](https://github.com/Nourishere/Zephyr_Tutorial/tree/main/examples/boards)
- [West Workspaces](notes/04_WestWorkspaces.md)

### Extras
- [Board Simulation Using Renode](notes/BONUS_BoardSimulationUsingRenode.md)
- [OpenOCD](notes/12_OpenOCD.md)

---

## Resources
1. [Practical Zephyr Series](https://interrupt.memfault.com/tags#practical-zephyr-series)
2. [Introduction To Zephyr: DigiKey](https://www.youtube.com/playlist?list=PLEBQazB0HUyTmK2zdwhaf8bLwuEaDH-52)
3. [Zephyr RTOS Official Documentation](https://docs.zephyrproject.org/latest/)
4. [Zephyr GitHub Repository](https://github.com/zephyrproject-rtos/zephyr)
