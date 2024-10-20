---
title: Resumen
author: Da Silva Sales, Marcelo Daniel
date: 2024-10-19
category: Jekyll
layout: post
---

Este trabajo presenta la prototipación de una solución para la gestión de dispositivos IoT aplicados al control de tráfico en ciudades inteligentes. La creciente cantidad de dispositivos IoT distribuidos en entornos urbanos impone desafíos significativos para la administración y actualización de estos equipos. La propuesta aquí presentada busca explorar el uso de dispositivos accesibles como el Raspberry Pi, que, debido a su capacidad computacional y bajo costo, permiten la implementación de soluciones robustas para la gestión automatizada de dispositivos de tráfico.

El proyecto parte de una configuración mínima de un Raspberry Pi, que tiene solo un agente instalado. A través de técnicas como Zero Touch, un conjunto de tareas automatizadas se encarga de instalar y configurar el software necesario para el funcionamiento de estos dispositivos. Para la gestión remota, se implementó un panel de control que permite tanto el envío de comandos como la monitorización en tiempo real del estado de los dispositivos.

La solución adopta una arquitectura basada en microservicios, lo que permite beneficios significativos en eficiencia y escalabilidad. Los servicios son más rápidos de iniciar y detener, proporcionando respuestas ágiles a los cambios en el entorno. Además, la naturaleza especializada de los microservicios permite que cada dispositivo consuma menos energía, ya que solo se activan los componentes necesarios. Otro beneficio es la capacidad de ejecutar una mayor cantidad de servicios especializados en los dispositivos, maximizando el uso de los recursos computacionales limitados. Este enfoque modular también facilita el mantenimiento y la actualización de los sistemas, permitiendo cambios en el software con mínima interrupción en las operaciones de los dispositivos, lo que es crucial en entornos de tráfico urbano donde la alta disponibilidad es esencial.

Se utilizaron herramientas como Ansible para la configuración inicial de los dispositivos, preparándolos para una autoconfiguración automática y segura. Además, se creó un entorno virtualizado que soporta una instalación de Kubernetes, responsable de gestionar todos los componentes del panel de control, garantizando una administración centralizada y eficiente.

Como estudio de caso, se configuraron dos dispositivos Raspberry Pi para simular un semáforo y un panel de velocidad. A través de la solución propuesta, se demuestra cómo el software en estos dispositivos puede actualizarse de forma remota con un tiempo de inactividad casi nulo y sin la necesidad de intervención humana directa. Este enfoque ofrece una solución eficiente y escalable para la gestión de dispositivos IoT en entornos urbanos, garantizando alta disponibilidad y flexibilidad para futuras expansiones.
