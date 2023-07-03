# AMBA specification
The Advanced Microcontroller Bus Architecture (AMBA) specification defines an on-chip communications standard for designing high-performance embedded 
microcontrollers. 
Three distinct buses are defined within the AMBA specification: 
• the Advanced High-performance Bus (AHB)
• the Advanced System Bus (ASB)
• the Advanced Peripheral Bus (APB).
A test methodology is included with the AMBA specification which provides an infrastructure for modular macrocell test and diagnostic access.


## 1 Advanced High-performance Bus (AHB)
The AMBA AHB is for high-performance, high clock frequency system modules. The AHB acts as the high-performance system backbone bus. AHB supports the 
efficient connection of processors, on-chip memories and off-chip external memory interfaces with low-power peripheral macrocell functions. AHB is also specified to ensure ease of use in an efficient design flow using synthesis and automated test 
techniques.

## 2 Advanced System Bus (ASB)
The AMBA ASB is for high-performance system modules.
AMBA ASB is an alternative system bus suitable for use where the high-performance 
features of AHB are not required. ASB also supports the efficient connection of 
processors, on-chip memories and off-chip external memory interfaces with low-power 
peripheral macrocell functions. 

## 3 Advanced Peripheral Bus (APB)
The AMBA APB is for low-power peripherals.AMBA APB is optimized for minimal power consumption and reduced interface 
complexity to support peripheral functions. APB can be used in conjunction with either version of the system bus

![image](https://github.com/shikhargovil/AHB-to-APB-Bridge/assets/78219141/89c8920e-fe85-4f9a-92b9-207f3dc63766)


# AHB-to-APB-Bridge
The AHB to APB bridge is an AHB slave, providing an interface between the high speed AHB and low power APB. Read and Write transfer of AHB are converted to equivalent transfer on the APB. As APB is not pipelined, then wait states are added during the transfers to and from the APB when AHB is required to wait for the APB.
![image](https://github.com/shikhargovil/AHB-to-APB-Bridge/assets/78219141/67ac5241-fe88-41f4-8a89-9f6ad0255eec)
                                              
Block Diagram of Bridge module


The main section of this module are:
1) AHB slave bus interface
2) APB transfer state machine
3) APB output signal generation
