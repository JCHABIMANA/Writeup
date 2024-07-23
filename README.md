# Challenge: IP - Time To Live
## IP:Internet Protocol
> Protocole informatique de connexion qui gère la transmission des données par internet.
## Adresse IP 
C'est un numéro d'identification d'un appareil connecté à un réseau informatique utilisant les protocole internet.
## Réseau informatique
> C'est un ensemble d'ordianateurs et dispositif connectés entre eux pour partager des ressources et des informations.
## Types de réseaux
LAN: Local Area Network(réseau local) comme un réseau d'un batiment ou une maison
WAN: Wide Area Network comme un réseau d'une ville, un pays ou du monde.
## Types d'adresse IP
 Adresse IP Public, adresse IP prive, adresse IP static, adresse IP dynamique.
## IPv4 vs IPv6
## Time To Live (Temps de vie)
C'est le temps pendant lequel une information doit etre conservée, ou le temps pendant lequel une information doit etre gardée en cache.
TTL fait référence à la durée ou nombre de sauts pendant lesquels un paquet est censé exister dans un réseau avant d'etre rejeter par un routeur.

## ANALYSE (source - destination)
Pour réaliser une étude source-destionation, je vais exploite les propriéte du couche réseau.
Sur la couche réseau il y a le protocole ICMP (Internet Control Message Protocol)
Je dois chercher une commande qui lie les deux bouts (source et destination)
## ICMP
C'est un protocole de couche réseau du model OSI, il est utilisé pour le rapport d'erreurs et les diagnostics dans les réseaux IP. 
PING envoie des message ICMP à l'appareil de destination pour verfier son accessibilité et mesurer le temps d'aller-retour.
Pour visualiser se qui se passe dans le réseau, il y a un autre outil qui s'appelle wireshark que j'aurai besoin
## WIRESHARK
C'est un analyseur de paquets qui est utilisé dans le dépannage et l’analyse de réseaux informatiques...
Je télécharge le logiciel et je l'installe pour visualiser mon réseau
## SOLUTIONS
Pour connaitre le TTL de mon challenge, je vais ouvrir le terminal de mon ordinateur je lance la commande ping IP_destination.
Je lance mon wireshark, avec une filtre ICMP puis je regarde le temps de demande (request) et le temps de reponse (reply) .
Ces deux paramètre vont m'aider à tirer la conclusion.
## Clonclusion
Le TTL=13






