# DHCP dns en dynamic route

Met dit bestand kun je op een overzichtelijke manier laten zien de functies van bijvoorbeeld een nsp en de functie van dns.

## Belangerijk
**Na het downloaden kan het zijn dat de ip adressen op een apipa (169.254.XXX.XXX) dan moet je even de tijd vooruit zetten en van static naar dhcp zetten op de pc,s.**

## Ip van devices
PC 0 192.168.10.30/24 DG 192.168.10.1 DNS server 192.168.201.1 DNS xiam

PC 1 192.168.10.31/24 DG 192.168.10.1 DNS server 192.168.201.1 DNS PCB

PC 2 192.168.20.30/24 DG 192.168.20.1 DNS server 192.168.201.1 DNS Ariva

PC 3 192.168.20.31/24 DG 192.168.20.1 DNS server 192.168.201.1 DNS NS

### DHCP server 192.168.200.2/24 DG 192.168.200.1 DNS server 192.168.201.2
Pool serverPool : DG 192.168.10.1 DNS server 192.168.201.2 Start ip 192.168.10.30/24
Pool 20 : DG 192.168.20.1 DNS server 192.168.201.2 Start ip 192.168.20.30/24
