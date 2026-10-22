#  Architecture Réseau d'Entreprise & Segmentation VLAN (Cisco)

**Auteur :** Nodem Nodem Luca Evans  
**Spécialité :** Génie Software, Réseaux & Sécurité — Keyce Informatique et IA

---

##  Présentation du Projet
Ce laboratoire présente la conception et le déploiement d'une infrastructure réseau locale (LAN) hautement disponible et sécurisée pour une entreprise, basée sur des équipements Cisco.

##  Concepts & Technologies
- **Commutation (Switching) :** VLANs, Trunking (802.1Q), VTP, Spanning Tree Protocol (STP)
- **Routage (Routing) :** Routage Inter-VLAN (Router-on-a-Stick / Switch N3)
- **Services Réseau :** DHCP Snooping, Port Security, ACLs (Access Control Lists)

##  Plan d'Adressage & VLANs
| VLAN ID | Nom du Réseau | Plage IP (Subnet) | Rôle |
| :--- | :--- | :--- | :--- |
| **VLAN 10** | ADMINISTRATION | `192.168.10.0/24` | Postes de gestion et serveurs |
| **VLAN 20** | EMPLOYES | `192.168.20.0/24` | Postes de travail utilisateurs |
| **VLAN 30** | INVTES / GUESTS | `192.168.30.0/24` | Accès Wi-Fi visiteurs isolé |
| **VLAN 99** | MANAGEMENT | `192.168.99.0/24` | Gestion distante des équipements |

## Sécurité Appliquée
- Isolation stricte du réseau Invités via des **ACLs Standard/Étendues**.
- Protection contre les attaques ARP Spoofing et serveurs DHCP roguish.
- Désactivation des ports non utilisés et association MAC via **Port Security**.
- 
