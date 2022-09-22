---
parent: Harmony 3 Wireless application examples for WINC1500/WINC3400
title: TCP Client
has_toc: true
has_children: false
has_toc: false
nav_order: 1

family: WINC
family: SAMA5D27
function: TCP Client
---

# TCP Client

The WINC example application demonstrates as a conventional, open tcp client-server communication.

## Description

In this demonstration, the WINC Driver will connect to a BSS and begin a TCP client socket connection to a remote server service.
This demonstration can be configured in the following ways in the source code.
• The BSS to connect to.
• The TCP server address and port to connect to.
• The receive buffer size.
• The message which should be sent as the first data once connected to the server.

## Downloading and building the application

To download or clone this application from Github, go to the [top level of the repository](https://bitbucket.microchip.com/projects/WSGSW/repos/wireless_wifi)


Path of the application within the repository is **apps/tcp_client/firmware** .

To build the application, refer to the following table and open the project using its IDE.

| Project Name      | Description                                    |
| ----------------- | ---------------------------------------------- |
| sam_a5d27_som1_winc1500.X | MPLABX project for SAMA5D27 and WINC1500 Xplained pro
| sam_a5d27_som1_winc3400.X | MPLABX project for SAMA5D27 and WINC3400 Xplained pro
|||


### Setting up [SAMA5D27-SOM1-EK1 Evaluation Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/atsama5d27-som1-ek1)

- Connect the Debug USB port on the SAMA5D27-SOM1-EK1 board to the computer using a micro USB cable
- Make sure to connect WINCxxxx XPRO with SAMA5D27-SOM1-EK1 board using Custom mikroBUS to XPRO adapter, WINCxxxx on MBus1.
#### Setting up the SD Card

- Download harmony MPU bootstrap loader from this [location](firmware/at91bootstrap_sam_a5d27_som1_ek.X/binaries/boot.bin)
- Copy the downloaded boot loader binary( boot.bin) onto the SD card
- Copy the application (harmony.bin) from "firmware/sam_a5d27_som1_winc3400.X/dist/sam_a5d27_som1_winc3400/production" onto the SD card, 
  available after a successful build of the application (Refer to the 'Running the Application' section below)

#### Setting up the board

- Insert the FAT32 formatted SD card with the boot.bin and harmony.bin (Refer to the 'Running the Application' section below) to J12
- Connecting a micro-USB cable to J10 both powers the board as well as provides a virtal COM port to open a serial terminal

## Running the Application

1. Open the project.
2. Build and program the generated code into the hardware using its IDE.
	 - Note: at91bootstrap_sam_a5d27_som1_ek.X project is linked to application project and is required to program the application on SAMA5D27-SOM1-EK1. 	 
3. Refer "firmware update guide" and "WINC Driver Demonstrations" for information.
4. To upgrade the firmware on WINC1500/WINC3400 
	 - use the Host SAMD21/SAME54 using serial_bridge application