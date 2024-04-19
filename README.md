# epsi-asrc-b2m2-tp2-projet


## Contexte

Vous rejoignez en alternance la société Best Network Inc., prestataire système et réseau dans la région grenobloise.

La société a été chargée de mettre en place la connexion réseau pour la future convention Grenobl'IT, qui va réunir des professionnels de l'informatique.

## Topologie

Le bâtiment retenu est composé d'une grande salle qui devra être couverte par du réseau sans-fil, d'une salle de conférence qui servira pour les conférences de presse, et de petits bureaux pour les organisateurs.

Pour des raisons de sécurité, il est nécessaire de différencier le réseau WiFi qui sera utilisé par les visiteurs du réseau Wifi utilisé par les conférenciers et exposants.

Pour permettre d'héberger les services locaux (AD, DNS, NAS, etc), un réseau dédié aux serveurs internes devra être configuré.
Enfin, pour les services mis à disposition des personnes (conférenciers et visiteurs) en distanciel, une DMZ devra être mise en place.
Pour des raisons de sécurité, la DMZ devra être reliée directement au routeur de bordure pour les flux entrants, et par un autre routeur pour accéder aux réseaux locaux.

## Volumétrie
 
Un total de 8'000 à 8500 visiteurs sont attendus chaque jour de la conférence
63 conférenciers se relaieront tout au long des 3 jours de la convention
150 stands ont été vendus ; cependant, chaque entreprise peut envoyer 1 ou 2 personnes pour la représenter
5 serveurs physiques internes sont prévus (un serveur physique qui hébergera l'AD, un DNS, et un serveur d'impression, un serveur d'authentification pour le WiFi, un serveur de fichiers, un serveur d'application et un serveur de bases de données)
2 serveurs physiques (pour un reverse-proxy/serveur visio et un serveur VPN) seront installés dans la DMZ


## Consignes :
 
- dimensionnez les réseaux au plus juste, afin de garder le maximum d'espace d'adressage disponible
-Choisissez vos réseaux afin de réduire le nombre de lignes dans les tables de routage des différents équipements
-préparez manuellement la table de routage d'un des routeurs de coeur de réseau ; configurez ensuite votre réseau sur Packet Tracer, activez RIP, et comparez la table que vous avez créée avec celle obtenue
préparez la matrice des flux réseau qui décrit l'ensemble des flux autorisés à transiter via les pare-feux qui seront mis en place durant l'évènement.
- sur Packet Tracer:
  - configurez un serveur DNS sur un des serveurs du réseau interne
  - configurez un serveur WEB dans la DMZ
  - configurez du DHCP sur le réseau
  - depuis une station de travail interne faites une résolution DNS et analysez les trames
  - depuis une station de travail interne faites une requete WEB et analysez les trames
