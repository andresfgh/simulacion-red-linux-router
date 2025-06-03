# 🛠️ Simulación de Red Interna con Linux y Alta Disponibilidad (2025)

Este repositorio documenta una práctica de Redes II de la Universidad Doctor Andrés Bello, donde se simuló una red interna utilizando máquinas virtuales (OVA), configuración de servidores Linux y topología en Cisco Packet Tracer.

---

## 🎯 Objetivo

Proporcionar una guía completa para la configuración de una red local con:

- Servidor DNS usando **BIND** en Rocky Linux.
- Servidores web usando **NGINX** (AlmaLinux) y **Apache2** (openSUSE Tumbleweed) con **failover** mediante **Keepalived**.
- Asignación de IP estática con Wicked/NetworkManager.
- Redundancia y alta disponibilidad usando una **IP virtual (VIP)**.
- Documentación detallada de retos y soluciones aplicadas.

---

## 🖥️ Componentes principales

- **DNS (BIND)** – Rocky Linux (`192.168.0.10`)
- **Web (NGINX)** – AlmaLinux (`192.168.0.5`)
- **Web Backup (Apache2)** – openSUSE Tumbleweed (`192.168.0.6`)
- **VIP con Keepalived** – `192.168.0.150`
- **Simulación de red** – Cisco Packet Tracer

---

## 📦 Tecnologías utilizadas

- Rocky Linux, AlmaLinux, openSUSE Tumbleweed
- BIND, NGINX, Apache2, Keepalived
- Cisco Packet Tracer
- FirewallD, Wicked, NetworkManager
- EPEL, net-tools

---

## 📁 Contenido del repositorio

| Carpeta/Archivo       | Descripción |
|-----------------------|-------------|
| `INFORME_MESA4.pdf`   | Documento formal del proyecto. |
| `ova/`                | Imágenes de máquinas virtuales exportadas. |
| `configuraciones/`    | Archivos de configuración de red, web, DNS y HA. |
| `capturas/`           | Imagen de la topología de red. |
| `packet-tracer/`      | Archivo `.pkt` con simulación lógica de la red. |

---

## 📷 Vista previa

![Topología de red](capturas/topologia_red.png)

---

## 📜 Instrucciones de uso

1. Importa las máquinas `.ova` en VirtualBox.
2. Asegúrate que estén en la misma red interna o puente.
3. Verifica IPs, servicios DNS y web con `ping` y navegador.
4. Simula una falla para comprobar el failover con Keepalived.

---

## 🛡️ Retos enfrentados

- Restricciones impuestas por el ISP en el router.
- Diferencias entre distribuciones (RHEL, openSUSE).
- Versiones de paquetes incompatibles (bind, nginx, apache2).

---

## 📖 Créditos

**Estudiantes:**  
- Richard Alexis Avalos Garcia  
- Ivania Nicole Hernandez Mendez  
- Rene Israel Rodriguez Palacios  
- Andres Felipe Galan Hernandez

---

## 📄 Licencia

Este proyecto se publica bajo la licencia [MIT](LICENSE).

