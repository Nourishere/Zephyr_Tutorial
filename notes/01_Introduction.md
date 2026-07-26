# Introduction to Zephyr
## Agenda
1. What is the Zephyr Project?
2. History
3. The Zephyr Kernel
4. The Zephyr SDK
5. West
6. Board Support
7. Resources

## What is the Zephyr Project?
* The Zephyr Project is an open-source collaborative project hosted by the [Linux Foundation](https://www.linuxfoundation.org/). The Zephyr project provides the Zephyr kernel, the Zephyr SDK, and West (the meta tool).

## History
| Year | Description |
| --- | ----------- |
| 1993 | Eonic System launch __Virtuoso__ as a DSP RTOS|
| 2001 | Wind River acquires Eonic Systems |
| 2015 | The project was renamed to **Rocket** and then open-sourced |
| 2016 | The Linux Foundation announces **Zephyr** (based on Rocket) |

* After the Linux Foundation announced Zephyr, big companies started joining the project. These include **Intel, Google, Texas Instruments, arm, Infinion, Qualcomm, and many more.**

## The Zephyr Kernel
* At the heart of the Zephyr Project is the Zephyr kernel. It provides the HW abstraction on which developers can extend. Zephyr supports many features including synchronization primitives, virtual memory, storage support, filesystem support, Logging, DSP, Networking, and more.
* Zephyr was originally designed as a microkernel[^1] on top of a nanokernel. However, after version 1.6, design changed to a pure monolithic kernel. This transition had the following merits:
    * The kernel became a single unified image with a single API, which was easier to configure and work with.
    * The unified kernel increased performance due to eliminated inter-kernel communication (between the nanokernel and the microkernel).
    * Overall reduced code footprint.

  ## The Zephyr SDK
  * Zephyr offers its own SDK, which is intended to work within the Zephyr ecosystem. This SDK includes GCC/LLVM compiler toolchain for all of Zephyr's supported architectures, the QEMU emulator, and OpenOCD.
  * Installing the Zephyr SDK is usually done using the **West** meta tool, which we'll come into later.

  ## West
  * West is Zephyr's Swiss army knife. It acts as an front-end interface on top of the various configuration tools and programs used in the Zephyr development.
  * West was originally designed to fill in the basic requirements that the Zephyr project needed at that time. These requirements were as follows:
    1. Keep externally maintained code in separate repos outside the main Zephyr repo.
    2. Provide a tool for both end users and downstream distributors. (generic and extensible).
    3. Allow the override of repositories without modifying the Zephyr repo.
    4. Support both continuous tracking and commit-based project updating.

  * In simple terms, Zephyr wanted a tool that could enable designers and developers to design applications that aren't necessarily part of the Zephyr mainline. At that time, **git** and Google's **repo** didn't satisfy these requirements.
  ## Board Support
  * As of August 2026, 1100+ boards are supported by Zephyr. This number is in continuous increase.
  * Because Zephyr is intended to provide a low footprint kernel, it is usually used in small boards with limited resources. Because it is an RTOS, its main concern is to provide a kernel that obeys real-time requirements.
  * Many of the boards that are intended for higher-end applications are not supported by Zephyr. These boards that have memory resources in the megabyte, or even the gigabyte, range are better coupled with sophisticated kernels like Linux. Note that most of these boards focus on **throughput** rather than being **real-time**.

  ## Resources
  * A good Zephyr introduction presentation: [https://www.zephyrproject.org/wp-content/uploads/2026/04/Zephyr-Overview-20260424.pdf]
  * Zephyr's supported boards: [https://docs.zephyrproject.org/latest/boards/index.html#]

    [^1]: A microkernel is a minimal kernel that provides the base OS functionalities and defers most others to userspace.
