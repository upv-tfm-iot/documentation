---
title: Architectural Diagrama
author: Da Silva Sales, Marcelo Daniel
date: 2024-10-19
category: Jekyll
layout: post
mermaid: true
---
## Architectural Diagrama
```mermaid
architecture-beta
    group m1[Macbook Pro M1]
    
    service controlplane(devicon:kubernetes)[VM Control Plane] in m1
    service k8sm(cloud)[Kubernetes Control Plane] 

```