# LockINetwork
> **L'approche narrative, pour progresser sur les modules CCNA, organisée autour de scénarios pratiques.**
---
## Philosophie
Chaque notion est introduite à partir d'un problème concret plutôt que dans l'abstrait : on part d'une topologie minimale (deux postes, un câble) et on complexifie uniquement quand la configuration précédente montre ses limites.
Aucun fichier Packet Tracer préconfiguré n'est fourni. Chaque niveau donne une matrice de connexion (port à port) ou capture d'écran de Packet Tracer et un plan d'adressage ; vous avez donc l'occasion de monter les labs vous-même sur Packet Tracer.

## Roadmap
Le découpage suit le cursus CCNA v7.0 (ITN, SRWE, ENSA) :

| Niveau | Sujet | Problème de départ | Solution technique | Module CCNA |
|---|---|---|---|---|
| 01 | Topologie de base | Échanger un fichier entre deux postes sans support physique | Câblage direct, switch | CCNA 1 – ITN |
| 02 | Boucle involontaire | Un second câble ajouté "pour la sécurité" paralyse tout le réseau | STP, rôles de port, PortFast | CCNA 2 – SRWE |
| 03 | Segmentation | Le trafic broadcast d'un seul service sature tous les postes | VLANs, ports d'accès | CCNA 2 – SRWE |
| 04 | Interconnexion | Deux switches, un seul câble : faire circuler plusieurs VLANs dessus | Trunking 802.1Q, VLAN natif | CCNA 2 – SRWE |
| 05 | Collaboration inter-services | Les VLANs sont étanches, mais deux départements doivent échanger des données | Routage inter-VLAN (router-on-a-stick) | CCNA 2 – SRWE |
| 06 | Résilience | Une seule panne de lien ou de passerelle coupe tout | EtherChannel, HSRP | CCNA 2 / CCNA 3 |
| 07 | Croissance du réseau | Les routes statiques deviennent ingérables à mesure que le réseau grandit | OSPF (aire unique) | CCNA 3 – ENSA |
| 08 | Ouverture externe | Le réseau interne doit accéder à Internet avec des adresses privées | NAT | CCNA 3 – ENSA |
| 09 | Chaos administratif | Heures désynchronisées, IP à configurer à la main, aucune alerte en cas de panne | DHCP, NTP, SNMP, Syslog | CCNA 2 / CCNA 3 |
| 10 | Intrusion non filtrée | N'importe quel poste atteint n'importe quel service, sans restriction | ACLs, port security | CCNA 2 – SRWE |
| 11 | Accès non contrôlé | Un mot de passe local unique partagé par tous les administrateurs | AAA, politiques de mot de passe, MFA | CCNA 3 – ENSA |
| 12 | Extension sans fil | Les nouveaux locaux n'ont pas de prises réseau | SSID, WLC, WPA2/3 | CCNA 2 / CCNA 3 |
| 13 | Épuisement IPv4 | Le pool d'adresses IPv4 disponible touche à sa fin | Adressage et cohabitation IPv6 | CCNA 1 – ITN |
| 14 | Configuration manuelle non scalable | Reconfigurer 50 switches un par un après chaque changement | APIs REST, JSON, Ansible/Terraform | CCNA 3 – ENSA |

## Structure d'un niveau
1. **Contexte** — le scénario qui amène le problème
2. **Objectifs** — ce qui doit être fonctionnel à la fin
3. **Topologie** — matrice de câblage et plan d'adressage
4. **Configuration** — commandes IOS utilisées

## Licence
MIT (2026). Scénarios et topologies sont des créations originales ; aucun fichier système Cisco ni document sous droit d'auteur n'est distribué ici.

*Un projet de vulgarisation de l'ingénierie réseau, en français.*
