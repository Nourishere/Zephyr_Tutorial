# Zephyr vs FreeRTOS
**FreeRTOS** 
- It is basically a scheduler with some syncronization primitives. 
- It has limited library support.
- It is lacking in overall flexibility.
- Developement relies on adding external libraries.

**Zephyr RTOS** 
- Has a modular, configurable design.
- Offers a rich set of subsystems and libraries.
- Has broad hardware support with over 790 (as of August 2025) and 1110 (as of August 2026) supported boards.
- Zephyr is a truly open-source project governed by [the Linux Foundation](https://www.linuxfoundation.org/) with a diverse and active community of contributors and sponsors.
* Here is a statement from the CTO of Nubix on why they ported from FreeRTOS to Zephyr.
> We decided to move from FreeRTOS to Zephyr for several reasons. First, we wanted to have a consistent and integrated platform for our devices, without having to manage multiple libraries and middleware. Zephyr has a comprehensive set of tools for managing dependencies, toolchains, and builds. Second, we wanted to leverage the benefits of Zephyr’s modern architecture, such as its scalability, flexibility, and reliability. Zephyr has a robust and secure kernel with support for multiple scheduling algorithms, memory protection, and fault handling. Third, we wanted to take advantage of Zephyr’s community and support. Zephyr is an open-source project, which means that we can contribute to its development and improvement.
## Advantages of Zephyr
- **Board Support**: 
	- Zephyr supports common architectures and instruction sets including ARM, x86, and RISC-V. There are currently more than 1110 community-supported boards from various architectures and vendors.
	- Unlike FreeRTOS, it leverages concepts from Linux such as Devicetree to make supporting new boards quick and easy.
- **Security and reliability**: 
	- It has a robust and secure kernel, which supports multiple scheduling algorithms, memory protection, and fault handling.
	- Zephyr also provides security features such as cryptography, secure boot, and firmware updates.
- **Driver libraries**: 
	- Zephyr includes built-in driver interfaces and libraries to support a lot of sensors and devices. This includes IP networking, wireless communications such as Wi-Fi, Bluetooth® and LoRaWAN®, as well as power management functionality to ensure long battery life.
- **Modularity and configurability**:
	- Zephyr is highly configurable and modular, allowing developers to customize it according to their needs and preferences. 
	- The Zephyr RTOS can run on devices with as little as 8 KB of RAM, and it can scale up to support complex applications and hardware.
- **Open source and community**:
	- Zephyr is an open source project backed by the Linux Foundation, which ensures its long-term sustainability and vendor-neutral governance.
	- The project has a vibrant and active community, which provides documentation, tutorials, forums, and mailing lists.
	
---
# Reference
- [Why We Moved from FreeRTOS to Zephyr RTOS – Zephyr Project](https://www.zephyrproject.org/why-we-moved-from-freertos-to-zephyr-rtos/)

#zephyr #embedded 
