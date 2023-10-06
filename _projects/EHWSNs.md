---
layout: page
title: EHWSNs
description: Energy Harvesting Powered Wireless Sensor Networks
img: assets/img/ehwsns/radiotest.png
importance: 3
category: Internet of Things
related_publications: 
---

This work involved the development of an Energy Harvesting platform for Internet of Things (IoT) based wireless sensor systems. It deals with the various intricacies and issues that come up during the integration of the various components that are developed by the lab for the purposes for of energy harvesting, storage, wireless radios. A bMote - (Berkeley Mote) platform was custom designed to enable low power operation, power management with dual reservoir (Battery and Supercapacitor) while harvesting energy from sources like Photovoltaics, Micro-wind turbines etc,. 

The below figure depicts how the different elements of the system interact with each other.  Initially, this was done using a Beta version TI Mote, however this was then shifted to a custom bult bMote. The platform hosts a Cascaded BQ25505 power management arrangement which is designed to perform stably for the varying voltage and power input from the various energy harvesting systems developed by the AME Lab. The module also extends its capability to be powered hybrid by any combination of super-capacitors, batteries (both printed and industrial variants) as well as using the raw power of the energy harvesting systems. The board is also capable of sensing the state as well as assessing the performance of the energy storage systems in order to facilitate changing its energy management schemes. The power management is capable of implementing various energy saving algorithms which can be programmed using the microcontroller (MCU) via a smartphone or the web. This is done through taking intelligent decisions of when, how and how long different elements of the platform are to powered and utilized. 

<b> Overview of the system </b>
<div style="background-color: white;">
<img src="/assets/img/ehwsns/overview.png" alt="Overview of the system" style="width: 100%; max-height: 300px; object-fit: contain;">
</div>


The platform is capable of communicating with a smartphone which acts a gateway for it to connect to an internet cloud. The board can be configured through the smartphone/web interface as well as the sensor data can be ported, visualized and analyzed on the cloud. The board is also designed taking into consideration that at a later stage, the MCU+BLE radio can be changed to an IC having ‘the state of the art’ wireless radio of that time. Currently, the ICs that are primarily being experimented with include nRF24L01 from Nordic Semiconductors and TI MSP432 from Texas Instruments. The research also looks into other competing radios as they come into the market. The power management of the platform is done by off-the-shelf components such as TI’s BQ25570 in combination with other passive elements. <b> The custom designed bMote and custom designed power board are shown below. </b> These were primarily tested with a PV panel and a Micro Wind Turbine.

<div style="background-color: white;">
<img src="/assets/img/ehwsns/inline_1.png" alt="Overview of the system" style="width: 100%; max-height: 300px; object-fit: contain;">
</div>

Subsequently, modelling some of the subsystems involved in the integration phase - the PV cell and an open-loop buck-boost converter as well as a simplified version of the sensor system. All the modelling was done in SIMULINK.

Modelling of PV Cell. In this, a PV panel simulator was developed in SIMULINK based on relations derived and established in the existing literature [1]. This enables us to develop I-V characteristic curves at different temperatures, irradiances, materials, geometric configurations using some data from the spec sheet of the solar panel like:

Material of the PV panel, Completion factor, Geometric config of cells, Reference data Irradiance, Reference data temp, Temperature coefficient of, Short circuit current, Short circuit Current, Open Circuit Voltage, Voltage at Pmax, Current at Pmax

The versatility of inputting so many parameters enables the simulator to simulate a very wide variety of solar cells that are available of market. Figure below shows the results of the developed SIMULINK model for simulating the solar panel, in comparison with experimental data provided in the manufacturer’s spec sheet of the solar panel used for powering the TI mote. We see that the simulated results closely match that of the experimental data. Using this, a maximum power point tracking (MPPT) system was simulated in the SIMULINK.

 

[1] - A detailed modeling method for photovoltaic cells - R. Chenni et. Al

<div style="background-color: white;">
<img src="/assets/img/ehwsns/simresults.jpeg" alt="Overview of the system" style="width: 100%; object-fit: contain;">
</div>