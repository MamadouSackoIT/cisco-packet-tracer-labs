# Lab Cisco Packet Tracer — Configuration d'un serveur DHCP

Ce laboratoire présente la mise en place d'un réseau local (LAN) avec **Cisco Packet Tracer**, comprenant un serveur DHCP, un switch et plusieurs postes clients.

L'objectif est de comprendre le fonctionnement du protocole **DHCP (Dynamic Host Configuration Protocol)** et de reproduire des tâches courantes d'un technicien systèmes et réseaux : configuration d'un serveur, attribution automatique d'adresses IP et vérification de la connectivité réseau.

## Environnement technique

- Simulateur : Cisco Packet Tracer
- Architecture : réseau local (LAN)
- Topologie : étoile
- Équipements : switch, serveur DHCP, PC et ordinateurs portables
- Protocole : DHCP
- Adressage IPv4 : 1.1.1.0/8
- Serveur DHCP : 1.1.1.1
- Plage d'attribution : à partir de 1.1.1.100
- Masque de sous-réseau : 255.0.0.0

---

## 1 — Création de la topologie réseau

Mise en place d'un réseau local composé de trois équipements principaux :

- Un serveur DHCP
- Un switch central
- Deux postes clients (PC0 et PC1)

Les équipements sont reliés au switch à l'aide de câbles Ethernet.

Cette architecture permet aux postes de communiquer sur le même réseau local.

## 2 — Configuration de l'adresse IP du serveur DHCP

Attribution d'une adresse IPv4 statique au serveur :

- Adresse IP : `1.1.1.1`
- Masque : `255.0.0.0`
- Interface : `FastEthernet0`

Cette adresse fixe permet au serveur de conserver une configuration réseau stable.

## 3 — Configuration du service DHCP

Activation du service DHCP depuis l'onglet **Services > DHCP** du serveur.

Configuration du pool d'adresses :

| Paramètre | Valeur |
|---|---|
| Nom du pool | serverPool |
| Adresse de début | 1.1.1.100 |
| Masque | 255.0.0.0 |
| Nombre maximal d'utilisateurs | 100 |
| Passerelle par défaut | 0.0.0.0 |
| Serveur DNS | 0.0.0.0 |

Le serveur peut ainsi attribuer automatiquement des paramètres IPv4 aux postes clients.

## 4 — Vérification de l'attribution DHCP sur PC1

Activation de l'option **DHCP** dans la configuration réseau du poste PC1.

Le poste reçoit automatiquement :

- Adresse IPv4 : `1.1.1.100`
- Masque : `255.0.0.0`

Cette étape permet de vérifier que le serveur DHCP distribue correctement une adresse IP.

## 5 — Vérification de l'attribution DHCP sur PC0

Réalisation du même test sur le second poste client.

Le poste PC0 reçoit :

- Adresse IPv4 : `1.1.1.101`
- Masque : `255.0.0.0`

Les deux postes disposent d'adresses distinctes attribuées automatiquement par le serveur DHCP.

## 6 — Validation de la topologie et des connexions

Extension du réseau avec plusieurs PC et ordinateurs portables connectés à un switch central.

Le serveur DHCP est également raccordé au switch.

Les indicateurs verts visibles sur les connexions permettent de vérifier que les interfaces réseau sont actives.

**Résultat :** la topologie est opérationnelle au niveau des liaisons physiques et les premiers tests confirment l'attribution automatique d'adresses IPv4 par DHCP.

---

## Compétences mises en pratique

Ce laboratoire m'a permis de travailler sur :

- Création et organisation d'un réseau local (LAN)
- Utilisation de Cisco Packet Tracer
- Compréhension d'une topologie en étoile
- Configuration IPv4 statique
- Configuration et activation d'un serveur DHCP
- Création d'un pool d'adresses DHCP
- Attribution automatique d'adresses IPv4
- Vérification des paramètres réseau des postes clients
- Identification de l'état des connexions réseau
- Compréhension du rôle d'un switch dans un LAN

---

## Objectif professionnel

Ce laboratoire s'inscrit dans ma montée en compétences en **administration systèmes et réseaux**.

Il me permet de consolider mes connaissances des fondamentaux réseau, notamment l'adressage IPv4, le fonctionnement du protocole DHCP et la configuration des équipements.

Ces compétences constituent une base pour évoluer vers des missions de technicien systèmes et réseaux, puis approfondir l'administration réseau et la cybersécurité.
