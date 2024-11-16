---
title: Architectural Diagram
subtitle: Subtitle
author: Da Silva Sales, Marcelo Daniel
date: 2024-10-19
category: Jekyll
layout: post
mermaid: true
---

### Device creation Process. Step 1
```mermaid
graph TD
    A[Start: Device Creation Process] --> B[Run Ansible Playbook]
    B --> C[Configure Agent]
    C --> D[Set Environment Variables]
    
    D --> VAR1[DEVICE_ID: Unique identifier of the device]
    D --> VAR2[DEVICE_TYPE: Type of the device]
    D --> VAR3[MQTT_COMMAND_IN_TOPIC: Topic for receiving commands]
    D --> VAR4[MQTT_COMMAND_OUT_TOPIC: Topic for sending command responses]
    D --> VAR5[MQTT_HUB_HOST: Hostname of the local MQTT hub]
    D --> VAR6[MQTT_HUB_LIVE_TOPIC: Topic for live communication]
    D --> VAR7[MQTT_HUB_PASS: Password for the MQTT hub]
    D --> VAR8[MQTT_HUB_PORT: Port of the MQTT hub]
    D --> VAR9[MQTT_HUB_USER: Username for the MQTT hub]
    D --> VAR10[ZONE: Zone to which the device belongs]
    
    D --> E[Agent Ready to Start]
    E --> F[Device Successfully Configured]
```

```mermaid
graph TD
    A[Configuração via Ansible Playbook] --> B[Configuração do Agente]
    B --> C[Parâmetros do Hub Local]
    C --> D[Variáveis de Ambiente Configuradas]
    
    D --> E[DEVICE_ID]
    D --> F[DEVICE_TYPE]
    D --> G[MQTT_COMMAND_IN_TOPIC]
    D --> H[MQTT_COMMAND_OUT_TOPIC]
    D --> I[MQTT_HUB_HOST]
    D --> J[MQTT_HUB_LIVE_TOPIC]
    D --> K[MQTT_HUB_PASS]
    D --> L[MQTT_HUB_PORT]
    D --> M[MQTT_HUB_USER]
    D --> N[ZONE]
```