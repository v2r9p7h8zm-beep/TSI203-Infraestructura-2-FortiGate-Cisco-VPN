# Topología – Infraestructura 2

La Infraestructura 2 fue desarrollada en GNS3 utilizando un
router Cisco y un firewall FortiGate conectados mediante una
red WAN/ISP simulada.

## Red USER

- Red: 10.86.0.0/25
- Gateway: 10.86.0.1
- PC-USER: 10.86.0.10
- VLAN: 10
- Asignación de dirección mediante DHCP

## Red WAN

- FortiGate: 200.20.86.1/30
- R-USER Cisco: 200.20.86.2/30

## Red SERVER

- Red: 10.86.1.0/28
- Gateway: 10.86.1.1
- PC-SERVER: 10.86.1.2

## VPN

La infraestructura utiliza una VPN IPsec Site-to-Site entre
el router Cisco y el FortiGate.

Durante la implementación se realizaron pruebas y
troubleshooting de la negociación IKE/IPsec, incluyendo
verificación de peers, propuestas criptográficas, ACL,
selectores y enrutamiento.
