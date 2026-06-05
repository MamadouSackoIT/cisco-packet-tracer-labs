# Mise en place d'un serveur DNS

## Objectif

Mettre en place un serveur DNS afin de permettre la résolution des noms des équipements présents sur le réseau.

## Technologies utilisées

- Cisco Packet Tracer
- DNS
- IPv4
- TCP/IP

## Topologie

![Topologie](topologie.png)

## Configuration du serveur DNS

Le serveur DNS a été configuré avec plusieurs enregistrements de type A :

| Nom | Adresse IP |
|------|------------|
| pc0 | 192.168.0.1 |
| pc1 | 192.168.0.2 |
| serveur_dns | 192.168.0.250 |

![Serveur DNS](serveur-dns.png)

## Configuration des postes clients

Les postes clients ont été configurés pour utiliser le serveur DNS :

Adresse du serveur DNS :

```text
192.168.0.250
```

### Configuration PC0

![PC0 DNS](pc0-config-dns.png)

### Configuration PC1

![PC1 DNS](pc1-config-dns.png)

## Vérification des adresses IP

### PC0

![Adresse PC0](pc0-adresse-ip.png)

### PC1

![Adresse PC1](pc1-adresse-ip.png)

## Tests de connectivité

### Ping depuis le serveur DNS

![Ping serveur](ping-serveur-vers-clients.png)

### Ping de PC1 vers PC0

![Ping PC1](ping-pc1-vers-pc0.png)

### Ping de PC0 vers PC1

![Ping PC0](ping-pc0-vers-pc1.png)

## Résultat

Le serveur DNS est opérationnel et les équipements du réseau peuvent communiquer correctement entre eux.

## Compétences développées

- Configuration DNS
- Résolution de noms
- Administration réseau
- Diagnostic réseau
- Cisco Packet Tracer
