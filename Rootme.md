# Challenge: IP - Time To Live
## IP:Internet Protocol
Protocole informatique de connexion qui gère la transmission des données par internet.
## Adresse IP 
C'est un numéro d'identification d'un appareil connecté à un réseau informatique utilisant les protocole internet.
## Réseau informatique
C'est un ensemble d'ordianateur et dispositif connectés entre eux pour partager des ressources et des informations.
## Types de réseaux
LAN: Local Area Network(réseau local) comme un réseau d'un batiment ou une maison
WAN: Wide Area Network comme un réseau d'une ville, un pays ou du monde.
## Types d'adresse IP
 Adresse IP Public, adresse IP prive, adresse IP static, adresse IP dynamique.
## IPv4 vs IPv6
IPv4: C'est la première version de protocole internet (1981) , elle est de 4 octets, 32 bits
IPv4:C'est la deuxème version de protocole internet (1998),elle est de 16 octets, 128 bits 

## Time To Live (Temps de vie)
C'est le temps pendant lequel une information doit etre conservée, ou le temps pendant lequel une information doit etre gardée en cache.
TTL fait référence à la durée ou nombre de sauts pendant lesquels un paquet est censé exister dans un réseau avant d'etre rejeter par un routeur.

## ANALYSE DU CHALLENGE (source - destination)
Pour réaliser une étude source-destination, je vais exploiter les propriétés du couche réseau.
Sur la couche réseau il y a le protocole ICMP (Internet Control Message Protocol)
Je dois chercher une commande qui lie les deux bouts (source et destination)

## ICMP
C'est un protocole de couche réseau du modèle OSI, il est utilisé pour le rapport d'erreurs et les diagnostics dans les réseaux IP. 
PING envoie des message ICMP à l'appareil de destination pour vérifier son accessibilité et mesurer le temps d'aller-retour.
Pour visualiser ce qui se passe dans le réseau, il y a un autre outil qui s'appelle Wireshark que j'aurai besoin

## WIRESHARK
C'est un analyseur de paquets qui est utilisé dans le dépannage et l’analyse de réseaux informatiques...
Je télécharge le logiciel et je l'installe pour visualiser mon réseau.

## PROCEDURE
- Je telecharger wireshark sur https://www.wireshark.org/download.html
- Je l'installe sur mon ordinateur IP_source (192.173.244.32)
- J'ouvre l'inviter de commandes sur mon ordinateur
- je lance la commande PING_IP destination (ping 24.6.126.218)
-  Je lance wireshark en filtrant ICMP
- ![Capture d’écran 2024-07-25 095708](https://github.com/user-attachments/assets/26bfb3a1-216a-4adf-9413-21a8ef128648)
- Par defaut, les valeurs TTL sont 64, 128, 254
- Pour verfier ma reponse TTL=64-reply TTL

## SOLUTIONS
Pour connaitre le TTL de mon challenge, je vais ouvrir le terminal de mon ordinateur je lance la commande ping IP_destination.
Je lance mon wireshark, avec une filtre ICMP puis je regarde le temps de demande (request) et le temps de reponse (reply) .
Ces deux paramètre vont m'aider à tirer la conclusion.
## Clonclusion
![Capture d’écran 2024-07-23 132236](https://github.com/user-attachments/assets/01dc2d64-4531-4931-aaae-cffd2a3cec59)

Le TTL=13

## CAPTURE DE FLAG

![FLAG](https://github.com/user-attachments/assets/b4e2c871-7ca7-4060-b6f0-c6e75d22c2d3)






