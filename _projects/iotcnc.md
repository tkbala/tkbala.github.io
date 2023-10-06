---
layout: page
title: IoT CNC Machine
description: IoT enabled CNC Milling machine
img: assets/img/iotcnc.png
importance: 1
category: Internet of Things
related_publications: kumaravel2017development
---

<b> Overview of the system </b>
<div style="background-color: white;">
<img src="/assets/img/iotcnc.png" alt="Overview of the system" style="width: 100%; max-height: 500px; object-fit: contain;">
</div>


This project was done during my time as a Visiting student working with Prof. Sanjay Sarma, Auto-ID Labs, MIT and as a final year student working with Prof. Arunachalam Narayanan and Prof. Balaraman Ravindran in IIT Madras.

"IoT enabled CNC Milling machine" won the best interdisciplinary thesis project amongst all engineering departments as well as the best thesis in Mechanical engineering. The project also won the gold medal in Aditya Birla Manufacturing summit 2016 held in Coimbatore, TN, India. The project was displayed in ACMEE  12th International Machine Tool Exhibition, where it received attention from the local press.

This work has  been presented at IEEE ROMA (Robotics and Manufacturing Automation) 2017 conference held in Kuala Lumpur, Malaysia

-----------------
<b> Context: </b>
Industry 4.0, (Industrie 4.0) which is termed as the fourth industrial revolution, encompasses broad fields of manufacturing, automation, machine to machine communications, and big data analytics. Having gone through the stages of Mechanization, Mass Production, Computer and Automation the industry is now moving towards an era where the boundary line between information technology and manufacturing is becoming thinner and thinner with the evolution of advanced cyber-physical systems. The aim of the concept is to achieve a ‘Smart Factory’. This involves the creation of a parallel ‘Virtual Factory’ alongside the physical one. The future of manufacturing would involve allotting jobs, controlling machines, analyzing machining data, monitoring machines and adapting machining real-time through using remote cloud services on the world wide web. The advantages of such a system are limitless. Possible applications include optimizing tool usage, predicting failures, enabling industry robot with more data and enabling direct to customer service.

----------------------

<b> Abstract: </b>
In this project, a model of an ‘IoT enabled manufacturing system’ has been developed and implemented. Various factors for designing the system architecture for such a system have been explored. The developed manufacturing system can take manufacturing inputs as G-Codes from the internet via a website as well as stream the data from different sensors to the internet. The project has implemented an open architecture control for the control of feed drives and open source hardware for its data acquisition system. Besides the core framework of the system, the project also explores the feasibility of using Micro Electro-Mechanical System (MEMS) based sensors for condition monitoring during manufacturing. This has been done using a test case research that was carried out on the developed manufacturing system. Its advantages and fallbacks have been analyzed and discussed in detail. Such a system will form as a primary unit in enabling the ‘Smart Factory’ revolution.

A feasibility analysis of using cheaper embedded Micro-Electro-Mechanical System (MEMS) for milling process over costlier industry grade sensors and a simple test case research was carried out on the developed platform. It is found that the MEMS accelerometer sensor is capable of substituting for an industry grade sensor. Savitzky-Golay filtering method was used to refine the frequency domain response of the accelerometer and optimal window size was found for maximizing the cross-correlation between the responses of MEMS MPU6050 accelerometer and the IEPE Dyatran 3145AG. Analysis was carried out to check for any correlations between wear and time domain parameters of accelerometer signals. The accelerometer signals were filtered using a butterworth low pass filter of 4th order. Though in this analysis, a correlation between wear and time domain parameters were not observed, it was found that there is a high correlation between time domain parameters of
both the accelerometers themselves.
