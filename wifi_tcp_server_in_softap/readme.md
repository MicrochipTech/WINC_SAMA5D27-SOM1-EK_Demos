---
parent: Harmony 3 Wireless application examples for WINC1500/WINC3400
title: TCP Server in SoftAP
has_toc: true
has_children: false
has_toc: false
nav_order: 1

family: SAMA5D27
function: TCP Server in SoftAP
---

# TCP Server in SoftAP

This example compiles the TCP Server in SoftAP application which is used to demonstrate a TCP Client-Server connection.

## Description

In this demonstration, the WINC Driver will advertise a SoftAP. The SoftAP connection is used to demonstrate a TCP client-server operation.

## Downloading and building the application

To download or clone this application from Github, go to the [top level of the repository](https://bitbucket.microchip.com/projects/WSGSW/repos/wireless_wifi)


Path of the application within the repository is **apps/wifi_tcp_server_in_softap/firmware** .

To build the application, refer to the following table and open the project using its IDE.

| Project Name      | Description                                    |
| ----------------- | ---------------------------------------------- |
| sam_a5d27_som1_winc1500.X | MPLABX project for SAMA5D27 and WINC1500 Xplained pro
| sam_a5d27_som1_winc3400.X | MPLABX project for SAMA5D27 and WINC3400 Xplained pro
|||


## Setting up SAMA5D27-SOM1-EK1 board

- Connect the Debug USB port on the SAMA5D27-SOM1-EK1 board to the computer using a micro USB cable
- Make sure to connect WINCxxxx XPRO with SAMA5D27-SOM1-EK1 board using Custom mikroBUS to XPRO adapter, WINCxxxx on MBus1.

## Running the Application

1. Open the project.
2. Build and program the generated code into the hardware using its IDE.
	 - Note: at91bootstrap_sam_a5d27_som1_ek.X project is linked to application project and is required to program the application on SAMA5D27-SOM1-EK1.
3. Refer "firmware update guide" and "WINC Driver Demonstrations" for information.
4. To upgrade the firmware on WINC1500/WINC3400 
	 - use the Host SAMD21/SAME54 using serial_bridge application
