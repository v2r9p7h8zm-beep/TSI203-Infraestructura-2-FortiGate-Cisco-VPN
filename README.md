# TSI-203 Seguridad de Redes
## Infraestructura 2 – VPN Site-to-Site FortiGate + Cisco

**Estudiante:** Jennifer López  
**Matrícula:** 20240860  

## 🎥 Video de demostración

🔗 **Enlace:** https://itlaedudo-my.sharepoint.com/:f:/g/personal/20240860_itla_edu_do/IgBqjRLpcY3YQLqFA3Ps6bXSAUA7cOwnBn79rRM6Q8jdicM?e=721vvY

---

## Objetivo

Implementar una infraestructura de Seguridad de Redes utilizando un
FortiGate y un router Cisco conectados mediante una VPN Site-to-Site.

La infraestructura permite la comunicación entre la red de usuarios
y la red de servidores a través de un túnel VPN.

## Características principales

- 1 FortiGate.
- 1 router Cisco.
- VPN Site-to-Site entre ambos peers.
- Red de usuarios /25.
- VLAN 10.
- DHCP.
- Red de servidores /28.
- Direccionamiento WAN público simulado.
- Enrutamiento entre las redes USER y SERVER.
- Pruebas y diagnóstico de conectividad.

## Direccionamiento

| Dispositivo | Interfaz | Dirección |
|---|---|---|
| R-USER | Fa0/0 | 200.20.86.2/30 |
| R-USER | LAN | 10.86.0.1/25 |
| PC-USER | VLAN 10 | 10.86.0.10/25 |
| FortiGate | port1 | 200.20.86.1/30 |
| FortiGate | port2 | 10.86.1.1/28 |
| PC-SERVER | LAN | 10.86.1.2/28 |

## VPN Site-to-Site

La VPN fue diseñada entre el router Cisco y el FortiGate utilizando
IPsec.

Parámetros principales:

- IKEv1
- DES
- SHA
- Diffie-Hellman Group 2
- IPsec Site-to-Site
- Autenticación mediante Pre-Shared Key

## Documentación

La documentación técnica completa de la infraestructura se encuentra
dentro de este repositorio.

## Configuraciones

La configuración correspondiente al router Cisco y al FortiGate se
encuentra en la carpeta `CONFIGURACIONES`.

## Evidencias y troubleshooting

El repositorio contiene las evidencias obtenidas durante la
implementación, incluyendo las pruebas de conectividad y el proceso
de diagnóstico realizado durante la configuración de la VPN.
