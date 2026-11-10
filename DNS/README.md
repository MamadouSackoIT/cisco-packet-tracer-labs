# 🌐 Laboratoire DNS – Cisco Packet Tracer

## 📌 Présentation du projet

Ce laboratoire consiste à mettre en place un **serveur DNS dans un réseau local** à l'aide de Cisco Packet Tracer.

L'objectif est de comprendre le fonctionnement du protocole DNS (Domain Name System), qui permet d'associer un nom d'hôte à une adresse IP afin de faciliter la communication entre les équipements.

## 🎯 Objectifs

- Créer un réseau local avec plusieurs équipements.
- Configurer un serveur DNS.
- Ajouter des enregistrements DNS de type A.
- Renseigner l'adresse du serveur DNS sur les postes clients.
- Vérifier la connectivité entre les équipements.

## 🛠️ Environnement technique

- **Logiciel :** Cisco Packet Tracer
- **Équipements :** 2 PC, 1 switch et 1 serveur
- **Protocole :** DNS
- **Adressage :** IPv4 statique
- **Tests :** commandes ping

## ⚙️ Configuration réalisée

### 1. Création du réseau local

Mise en place d'une topologie comprenant deux postes clients, un commutateur et un serveur DNS.

Les équipements sont reliés au switch afin de permettre leur communication sur le même réseau local.

### 2. Configuration de l'adressage IPv4

| Équipement | Adresse IPv4 |
|---|---|
| PC0 | 192.168.0.1 |
| PC1 | 192.168.0.2 |
| Serveur DNS | 192.168.0.250 |

Masque de sous-réseau : **255.255.255.0 (/24)**

### 3. Configuration du serveur DNS

Activation du service DNS sur le serveur et création des enregistrements de type A.

| Nom DNS | Adresse IPv4 |
|---|---|
| pc0 | 192.168.0.1 |
| pc1 | 192.168.0.2 |
| serveur_dns | 192.168.0.250 |

Ces enregistrements permettent d'associer les noms des équipements à leurs adresses IP.

### 4. Configuration des postes clients

Configuration de l'adresse du serveur DNS sur les deux postes :

**Serveur DNS : 192.168.0.250**

Les postes peuvent ainsi interroger le serveur pour résoudre les noms configurés.

### 5. Vérification de la connectivité

Réalisation de tests de connectivité avec la commande `ping` :

- PC0 vers PC1 : communication réussie.
- PC1 vers PC0 : communication réussie.
- Serveur vers PC0 : communication réussie.
- Serveur vers PC1 : communication réussie.

Les tests confirment que les équipements communiquent correctement sur le réseau local.

## ✅ Résultats et compétences acquises

Ce laboratoire m'a permis de travailler sur :

- La compréhension du fonctionnement du **DNS**.
- La configuration d'un **serveur DNS**.
- La création d'enregistrements **DNS de type A**.
- La configuration réseau des postes clients.
- Le diagnostic de connectivité avec **ping**.

Le réseau local est opérationnel et les enregistrements DNS sont configurés.

*Note : les captures valident la connectivité IP et la configuration DNS. Un test par nom d'hôte permettrait de confirmer également la résolution DNS.*

---

**Projet personnel réalisé dans le cadre de ma reconversion vers les métiers des systèmes et réseaux.**
