---
parent: Harmony 3 Wireless application examples for WINC1500/WINC3400
title: Wifi Provisioning via WPS
has_toc: true
has_children: false
has_toc: false
nav_order: 1

family: SAMA5D27
function: Wifi Provisioning via WPS
---

# Wifi Provisioning via WPS

This example compiles the Wifi Provisioning via WPS application which is used to provision a WiFi connection.

## Description

In this demonstration, the WINC Driver will move into WPS mode – PIN or PBC. By activating the WPS mode in the AP concurrently, a WiFi connection is established.

## Downloading and building the application

To download or clone this application from Github, go to the [top level of the repository](https://bitbucket.microchip.com/projects/WSGSW/repos/wireless_wifi)


Path of the application within the repository is **apps/wifi_provisioning_via_wps/firmware** .

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
3. Please refer "WINC Firmware Update Guide" and "WINC Driver Demonstrations" for more information.
4. To upgrade the firmware on WINC1500/WINC3400 
	 - use the Host SAMD21/SAME54 using serial_bridge application