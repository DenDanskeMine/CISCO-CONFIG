# Netværkskonfigurationsdokumentation

Dette dokument beskriver R1-1
## Interfaces

### Gi0/1.10 - VLAN 10
- **Beskrivelse:** VLAN 10 - fa0/1-12 på SW1
- **IP-adresse:** 172.16.0.3/26
- **Standby:** 172.16.0.1
- **Priority:** 110
- **Track:** Gi0/0, FastEthernet0/1/0
- **NAT:** Inde

### Gi0/1.20 - VLAN 20
- **Beskrivelse:** VLAN 20 - fa0/13-22 på SW1
- **IP-adresse:** 172.16.0.67/26
- **Standby:** 172.16.0.65
- **Priority:** 110
- **Track:** Gi0/0, FastEthernet0/1/0
- **NAT:** Inde

### Gi0/1.30 - VLAN 30
- **Beskrivelse:** VLAN 30 - fa0/1-12 på SW2
- **IP-adresse:** 172.16.0.131/26
- **Standby:** 172.16.0.129
- **Priority:** 110
- **Track:** Gi0/0, FastEthernet0/1/0
- **NAT:** Inde

### Gi0/1.40 - VLAN 40
- **Beskrivelse:** VLAN 40 - INTERN-WIFI
- **IP-adresse:** 172.16.1.3/25
- **Standby:** 172.16.1.1
- **Priority:** 110
- **Track:** Gi0/0, FastEthernet0/1/0
- **NAT:** Inde

### Gi0/1.50 - VLAN 50
- **Beskrivelse:** VLAN 50 - EKSTERN-WIFI
- **IP-adresse:** 172.16.1.131/25
- **Standby:** 172.16.1.129
- **Priority:** 110
- **Track:** Gi0/0, FastEthernet0/1/0
- **NAT:** Inde

### Fa0/1/0 - SW-mellemforbindelse
- **Beskrivelse:** SW mellem Sites /28
- **IP-adresse:** 10.10.10.3/28
- **Standby:** 10.10.10.1
- **Priority:** 110
- **Track:** Gi0/0, FastEthernet0/1/0
- **NAT:** Inde

## DHCP-pools

- VLAN10: 172.16.0.0/26
- VLAN20: 172.16.0.64/26
- VLAN30: 172.16.0.128/26
- VLAN40: 172.16.1.0/25
- VLAN50: 172.16.1.128/25

## OSPF Routing

- **Router ID:** 1.1.1.1
- **Netværk:** 172.16.0.0/26
- **Netværk:** 172.16.0.64/26
- **Netværk:** 172.16.0.128/26
- **Netværk:** 10.10.10.0/28
- **Netværk:** 172.16.1.0/25

## NAT Oversættelse

- Inde: Gi0/1.10, Gi0/1.20, Gi0/1.30, Gi0/1.40, Gi0/1.50

## Sikkerhed

- SSH adgang er konfigureret på VTY linjer
- Adgangskoder og nøgler er implementeret
- Sikkerhedsovervejelser som IP-spoofing er taget i betragtning

## Konklusion

Pisse nice konfig