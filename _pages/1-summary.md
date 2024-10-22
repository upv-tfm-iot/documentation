---
title: Resumen and Abstract
author: Da Silva Sales, Marcelo Daniel
date: 2024-10-19
category: Jekyll
layout: post
---

# Resumen

Este trabajo presenta la prototipación de una solución para la gestión de dispositivos IoT aplicados al control de tráfico en ciudades inteligentes. La creciente cantidad de dispositivos IoT distribuidos en entornos urbanos impone desafíos significativos para la administración y actualización de estos equipos. La propuesta aquí presentada busca explorar el uso de dispositivos accesibles como el Raspberry Pi, que, debido a su capacidad computacional y bajo costo, permiten la implementación de soluciones robustas para la gestión automatizada de dispositivos de tráfico.

El proyecto parte de una configuración mínima de un Raspberry Pi, que tiene solo un agente instalado. A través de técnicas como Zero Touch, un conjunto de tareas automatizadas se encarga de instalar y configurar el software necesario para el funcionamiento de estos dispositivos. Para la gestión remota, se implementó un panel de control que permite tanto el envío de comandos como la monitorización en tiempo real del estado de los dispositivos.

La solución adopta una arquitectura basada en microservicios, lo que permite beneficios significativos en eficiencia y escalabilidad. Los servicios son más rápidos de iniciar y detener, proporcionando respuestas ágiles a los cambios en el entorno. Además, la naturaleza especializada de los microservicios permite que cada dispositivo consuma menos energía, ya que solo se activan los componentes necesarios. Otro beneficio es la capacidad de ejecutar una mayor cantidad de servicios especializados en los dispositivos, maximizando el uso de los recursos computacionales limitados. Este enfoque modular también facilita el mantenimiento y la actualización de los sistemas, permitiendo cambios en el software con mínima interrupción en las operaciones de los dispositivos, lo que es crucial en entornos de tráfico urbano donde la alta disponibilidad es esencial.

Se utilizaron herramientas como Ansible para la configuración inicial de los dispositivos, preparándolos para una autoconfiguración automática y segura. Además, se creó un entorno virtualizado que soporta una instalación de Kubernetes, responsable de gestionar todos los componentes del panel de control, garantizando una administración centralizada y eficiente.

Como estudio de caso, se configuraron dos dispositivos Raspberry Pi para simular un semáforo y un panel de velocidad. A través de la solución propuesta, se demuestra cómo el software en estos dispositivos puede actualizarse de forma remota con un tiempo de inactividad casi nulo y sin la necesidad de intervención humana directa. Este enfoque ofrece una solución eficiente y escalable para la gestión de dispositivos IoT en entornos urbanos, garantizando alta disponibilidad y flexibilidad para futuras expansiones.


<b>Palabras clave:</b>  IoT, ciudades inteligentes, gestión de tráfico urbano, Raspberry Pi, Zero Touch, automatización, microservicios, Kubernetes, Ansible, Quarkus, panel de control remoto, actualización automatizada, arquitectura de contenedores, alta disponibilidad, dispositivos de tráfico

---

# Abstract

This work presents the prototyping of a solution for the management of IoT devices applied to traffic control in smart cities. The increasing number of IoT devices distributed in urban environments imposes significant challenges for the management and updating of these devices. The proposal presented here seeks to explore the use of accessible devices such as the Raspberry Pi, which, due to their computational capacity and low cost, allow the implementation of robust solutions for the automated management of traffic devices.

The project starts from a minimal configuration of a Raspberry Pi, which has only one agent installed. Through techniques such as Zero Touch, a set of automated tasks is responsible for installing and configuring the software necessary for the operation of these devices. For remote management, a control panel was implemented that allows both the sending of commands and the real-time monitoring of the status of the devices.

The solution adopts a microservices-based architecture, allowing significant benefits in efficiency and scalability. Services are faster to start and stop, providing agile responses to changes in the environment. Furthermore, the specialized nature of microservices allows each device to consume less power, as only the necessary components are activated. Another benefit is the ability to run a larger number of specialized services on the devices, maximizing the use of limited computational resources. This modular approach also makes it easier to maintain and update the systems, allowing for software changes with minimal disruption to device operations, which is crucial in urban traffic environments where high availability is essential.

Tools such as Ansible were used for the initial configuration of the devices, preparing them for automatic and secure self-configuration. In addition, a virtualized environment was created supporting a Kubernetes installation, responsible for managing all the dashboard components, ensuring centralized and efficient administration.

As a case study, two Raspberry Pi devices were configured to simulate a traffic light and a speed dashboard. Through the proposed solution, it is demonstrated how the software on these devices can be remotely updated with almost zero downtime and without the need for direct human intervention. This approach offers an efficient and scalable solution for managing IoT devices in urban environments, ensuring high availability and flexibility for future expansion.

<b>Keywords:</b> IoT, smart cities, urban traffic management, Raspberry Pi, Zero Touch, automation, microservices, Kubernetes, Ansible, Quarkus, remote control panel, automated update, container architecture, high availability, traffic devices