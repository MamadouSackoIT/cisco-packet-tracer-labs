# Communication entre deux réseaux via un routeur

## Objectif

Mettre en place une communication entre deux réseaux distincts à l'aide d'un routeur Cisco.

## Technologies utilisées

- Cisco Packet Tracer
- Routeur Cisco ISR4331
- Switch Cisco 2960
- IPv4
- TCP/IP

## Topologie

![Topologie](topologie.png)

Le laboratoire est composé :

- d'un réseau 192.168.0.0/24
- d'un réseau 192.168.100.0/24
- d'un routeur assurant l'interconnexion
- de plusieurs postes clients
- de serveurs présents sur chaque réseau

## Configuration du routeur

### Interface réseau gauche

- Adresse IP : 192.168.0.254
- Masque : 255.255.255.0

![Interface gauche](routeur-reseau-gauche.png)

### Interface réseau droite

- Adresse IP : 192.168.100.254
- Masque : 255.255.255.0

![Interface droite](routeur-reseau-droite.png)

## Configuration des passerelles par défaut

### Réseau 192.168.0.0/24

Passerelle :

```text
192.168.0.254
```

![Gateway gauche](gateway-reseau-gauche.png)

### Réseau 192.168.100.0/24

Passerelle :

```text
192.168.100.254
```

![Gateway droite](gateway-reseau-droite.png)

## Vérification de la connectivité

### Tests depuis le réseau 192.168.0.0

![Ping gauche](ping-reseau-gauche.png)

### Tests depuis le réseau 192.168.100.0

![Ping droite](ping-reseau-droite.png)

## Résultat

Les équipements appartenant aux deux réseaux peuvent communiquer grâce au routeur qui assure le routage entre les sous-réseaux.

## Démonstration vidéo

Une démonstration vidéo est disponible dans le dépôt afin de visualiser le transfert de paquets entre les deux réseaux.

## Compétences développées

- Configuration d'interfaces réseau
- Adressage IPv4
- Configuration de passerelles par défaut
- Routage inter-réseaux
- Diagnostic réseau
- Cisco Packet Tracer
