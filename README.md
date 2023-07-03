# AHB-to-APB-Bridge
The AHB to APB bridge is an AHB slave, providing an interface between the high speed AHB and low power APB. Read and Write transfer of AHB are converted to equivalent transfer on the APB. As APB is not pipelined, then wait states are added during the transfers to and from the APB when AHB is required to wait for the APB.
![image](https://github.com/shikhargovil/AHB-to-APB-Bridge/assets/78219141/67ac5241-fe88-41f4-8a89-9f6ad0255eec)
                  Block Diagram of Bridge module
