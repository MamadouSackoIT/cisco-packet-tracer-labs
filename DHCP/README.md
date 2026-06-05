# Configuration d'un réseau DHCP

## Objectif

Mettre en place un serveur DHCP afin d'attribuer automatiquement des adresses IP aux postes clients du réseau.

## Topologie

![Topologie](topologie.png)

## Configuration du serveur DHCP

Le serveur DHCP a été configuré avec les paramètres suivants :

- Réseau : 1.0.0.0/8
- Adresse de départ : 1.1.1.100
- Nombre maximal d'utilisateurs : 100

![Configuration DHCP](serveur-dhcp.png)

## Vérification des postes clients

### PC0

Adresse IP attribuée automatiquement :

![PC0](pc0-dhcp.png)

### PC1

Adresse IP attribuée automatiquement :

![PC1](pc1-dhcp.png)

## Résultat

Les postes clients obtiennent automatiquement une adresse IP grâce au serveur DHCP.

## Compétences développées

- Configuration DHCP
- Adressage IPv4
- Administration réseau
- Diagnostic de connectivité
- Cisco Packet Tracer
