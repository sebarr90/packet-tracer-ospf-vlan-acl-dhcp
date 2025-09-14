# packet-tracer-ospf-vlan-acl-dhcp
Configuraciones de rutas dinamicas, ACLs, DHCP

# Packet Tracer - OSPF, VLANs, ACLs y DHCP

## Descripción

Este proyecto es una simulación de red desarrollada en Cisco Packet Tracer. La topología incluye tres routers interconectados y varias VLANs, con las siguientes configuraciones:

- **Rutas dinámicas:** Se utiliza OSPF como protocolo de enrutamiento dinámico para intercambiar información de rutas entre los routers.
- **VLANs y subinterfaces:** Cada router tiene subinterfaces configuradas con 802.1Q para diferentes VLANs (VLAN 10, 20, 30 y 40).
- **ACLs (Listas de Control de Acceso):** Se implementan ACLs estándar y extendidas para controlar el tráfico entre redes y restringir el acceso a internet en ciertos casos.
- **DHCP:** El servidor (R3) distribuye direcciones IP automáticamente a las VLANs, excluyendo ciertas IPs fijas para routers y dispositivos críticos.
- **Rutas estáticas de respaldo:** Además de OSPF, se configuran rutas estáticas hacia redes externas.

Este ejercicio permite practicar los conceptos de enrutamiento dinámico, segmentación de redes mediante VLANs, control de acceso con ACLs y asignación automática de direcciones IP con DHCP.

---

## Configuraciones principales

### R1
- VLANs 10 y 20  
- OSPF ID: 1.1.1.1  
- ACL estándar 100 y extendida BLOQUEO_INTERNET  
- IP helper hacia R3 para DHCP  

### R2
- VLANs 30 y 40  
- OSPF ID: 2.2.2.2  
- ACL estándar 101  
- IP helper hacia R3 para DHCP  

### R3
- Servidor DHCP  
- VLANs 10, 20 y 30  
- Rutas estáticas hacia redes externas  

---

## Propósito del proyecto

El objetivo es **simular y practicar una red empresarial pequeña** que incluya:

- Segmentación de red con VLANs  
- Enrutamiento dinámico con OSPF  
- Control de tráfico con ACLs  
- Distribución automática de IPs mediante DHCP  
- Configuración de rutas estáticas como respaldo  

---

## Archivos incluidos

- Topología Packet Tracer (`.pkt`)  

---

## Autor

Marcos Arriagada Sáez  
Santiago, Chile
