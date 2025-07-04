---
layout: default
title: Wazuh
---


# Plan de Trabajo: Implementación de SIEM con Wazuh

## 🎯 Objetivo General

Implementar una solución SIEM basada en Wazuh para monitorear, analizar y detectar eventos de seguridad generados por 25 estaciones de trabajo (agentes) ubicadas en el laboratorio A de la Facultad de Ingeniería en Sistemas Computacionales.

---

## 🧩 Fase 1: Planificación

**Duración estimada:** 1 semana

**Actividades:**
- Levantar los requerimientos técnicos y operativos del entorno de laboratorio, incluyendo infraestructura física, red, sistema operativo y políticas de uso.
- Seleccionar la distribución del sistema operativo para el servidor SIEM. Se recomienda Ubuntu Server 22.04 LTS por su estabilidad y soporte a largo plazo.
- Validar la conectividad de red entre el servidor Wazuh y las 25 estaciones de trabajo que actuarán como agentes.
- Establecer roles de operación para la administración del SIEM durante su uso académico.

---

## 🛠️ Fase 2: Implementación Técnica

**Actividades:**
- Instalar y configurar el servidor Wazuh con sus componentes principales: Wazuh Manager, Elasticsearch y Kibana.
- Asignar una dirección IP fija al servidor para garantizar su disponibilidad en la red.
- Asegurar acceso al servidor tanto de forma física como remota (SSH).
- Generar una imagen de respaldo (snapshot) de la configuración base del servidor.
- Instalar el agente Wazuh en cada una de las 25 estaciones de trabajo.
- Verificar la comunicación exitosa entre los agentes y el servidor SIEM.

---

## 🔍 Fase 3: Configuración de Monitoreo y Reglas

**Actividades:**
- Definir políticas básicas de monitoreo como registro de eventos del sistema, autenticaciones y verificación de integridad de archivos.
- Activar módulos adicionales de análisis como Syscollector y Rootcheck.
- Personalizar reglas de detección de amenazas según los objetivos pedagógicos del laboratorio.
- Ejecutar pruebas de alerta mediante simulación de eventos sospechosos o ataques.

---

## 📘 Fase 4: Capacitación y Manuales

**Actividades:**
- Elaborar manuales de usuario para estudiantes y docentes sobre el uso básico del SIEM.
- Realizar sesiones prácticas de interpretación de alertas y análisis de incidentes.
- Diseñar ejercicios guiados que simulen escenarios de ataque y defensa en entornos controlados.

---

## 🧪 Fase 5: Evaluación y Ajustes Finales

**Actividades:**
- Simular incidentes para verificar la efectividad de la detección y respuesta del sistema.
- Ajustar reglas, políticas y configuraciones en función de los resultados observados.
- Establecer un procedimiento de mantenimiento periódico del sistema (mensual).

---

## 🖥️ Requerimientos Técnicos del Servidor

- CPU: 4 núcleos
- RAM: 8–16 GB
- Disco: 100–200 GB SSD
- Sistema Operativo: Ubuntu Server 22.04

---

## 📦 Entregables del Proyecto

- Servidor Wazuh funcionando con interfaz web accesible.
- Documentación técnica del servidor y credenciales iniciales.
- 25 agentes conectados y reportando al Wazuh Manager.
- Registro de instalación por cada máquina (hostname, IP, OS, etc.).
- Manual de usuario y presentación para capacitación.
- Dos prácticas educativas con objetivos, instrucciones y criterios de evaluación.
- Informe de evaluación final y plan de mantenimiento.

---

## 🗂️ Recursos Requeridos

| Recurso             | Cantidad | Descripción                                           |
|---------------------|----------|-------------------------------------------------------|
| Servidor físico o VM| 1        | Con especificaciones recomendadas para SIEM          |
| PCs o VMs cliente   | 25       | Estaciones de trabajo conectadas en red LAN          |
| Red local           | 1        | Con acceso bidireccional entre agentes y servidor    |
| Personal técnico    | 1–2      | Responsables de instalación, pruebas y soporte       |
| Documentación oficial| -       | https://documentation.wazuh.com                      |

