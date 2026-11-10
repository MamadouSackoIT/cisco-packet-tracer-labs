# 🌐 Laboratoire Routage & Switching – Cisco Packet Tracer

## 📌 Présentation du projet

Ce laboratoire consiste à mettre en place **deux réseaux locaux distincts**, interconnectés à l'aide d'un routeur Cisco dans Packet Tracer.

L'objectif est de comprendre le fonctionnement du **switching (commutation)** et du **routage inter-réseaux**, afin de permettre la communication entre des équipements appartenant à différents sous-réseaux.

## 🎯 Objectifs

- Créer deux réseaux locaux (LAN).
- Connecter les équipements à des switches.
- Configurer les interfaces d'un routeur Cisco.
- Définir les adresses IP et les passerelles par défaut.
- Permettre la communication entre deux sous-réseaux.
- Vérifier la connectivité avec la commande `ping`.

## 🛠️ Environnement technique

- **Logiciel :** Cisco Packet Tracer
- **Équipements :** 1 routeur Cisco, 2 switches, 2 serveurs et plusieurs PC fixes et portables
- **Protocoles :** IPv4, ICMP et Ethernet
- **Adressage :** IPv4 statique
- **Tests :** commandes ping

## ⚙️ Configuration réalisée

### 1. Création de la topologie réseau

Mise en place de deux réseaux locaux comprenant chacun plusieurs postes utilisateurs, un serveur et un switch.

Les deux switches sont connectés à un routeur central qui assure la communication entre les sous-réseaux.

### 2. Configuration des sous-réseaux

| Paramètre | Réseau 1 | Réseau 2 |
|---|---|---|
| Adresse réseau | 192.168.0.0/24 | 192.168.100.0/24 |
| Masque | 255.255.255.0 | 255.255.255.0 |
| Passerelle | 192.168.0.254 | 192.168.100.254 |

### 3. Configuration du routeur

Configuration des interfaces GigabitEthernet du routeur Cisco :

- **GigabitEthernet0/0/0 :** 192.168.0.254/24
- **GigabitEthernet0/0/1 :** 192.168.100.254/24

Le routeur permet d'acheminer les paquets entre les deux réseaux directement connectés.

### 4. Configuration des postes clients

Attribution des adresses IPv4 aux équipements et configuration des passerelles par défaut.

Chaque poste utilise l'adresse de l'interface du routeur correspondant à son réseau local.

### 5. Vérification de la connectivité

Réalisation de tests avec la commande `ping` depuis différents équipements :

- Communication entre les postes d'un même réseau.
- Communication entre des équipements de réseaux différents.
- Vérification des échanges entre les postes et les serveurs.

Les captures montrent des réponses ICMP positives entre les deux sous-réseaux.

Certains premiers tests présentent une perte ponctuelle de paquet, suivie de réponses réussies.

## ✅ Résultats et compétences acquises

Ce laboratoire m'a permis de travailler sur :

- La compréhension du **switching et du routage**.
- La création et l'interconnexion de **deux LAN**.
- La configuration des **interfaces d'un routeur Cisco**.
- L'adressage IPv4 et les **masques de sous-réseau**.
- La configuration des **passerelles par défaut**.
- Le diagnostic réseau avec **ICMP et ping**.

**Résultat :** les deux réseaux locaux peuvent communiquer grâce au routeur Cisco. Les tests réalisés confirment le fonctionnement du routage inter-réseaux.

---

**Projet personnel réalisé dans le cadre de ma reconversion vers les métiers des systèmes et réseaux.**
