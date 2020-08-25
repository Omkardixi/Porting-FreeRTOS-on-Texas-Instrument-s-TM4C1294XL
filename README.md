# Porting-FreeRTOS-on-Texas-Instrument-s-TM4C1294XL #

Operating System : FreeRTOS
IDE              : Keil uVision5
Terminal         : Hercules 3.2.8 

Requirements     : SOFTWARE DEVELOPMENT KITS (SDK) link: (https://www.ti.com/tool/SW-TM4C)  

Basically here I tried to perform UART operation. This example demonstrates 
the use of a UART port in loopback mode.  On being enabled in loopback mode, the transmit 
line of the UART is internally connected to its own receive line.  Hence, the UART 
port receives back the entire data it transmitted.

This example echoes data sent to the UART's transmit FIFO back to the same
UART's receive FIFO.  To achieve this, the UART is configured in loopback
mode.  In the loopback mode, the Tx line of the UART is directly connected
to its Rx line internally and all the data placed in the transmit buffer is
internally transmitted to the Receive buffer.

This example uses the following peripherals and I/O signals.  You must
review these and change as needed for your own board.
- UART7 peripheral - For internal Loopback
- UART0 peripheral - As console to display debug messages.
- UART0RX - PA0
- UART0TX - PA1

UART parameters for the UART0 and UART7 port:
- Baud rate - 115,200
- 8-N-1 operation

Note****
After sending the data user is expected to enter '@' at last.

Thank You!
