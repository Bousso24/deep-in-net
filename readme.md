# DEEP-IN-NET

## Objectif:
deep-in-net est un projet d'initiation aux réseaux informatiques utilisant Cisco Packet Tracer. En tant qu'étudiant DevOps/Cloud, tu vas apprendre les bases fondamentales du networking qui sont essentielles pour comprendre comment les systèmes communiquent.

### Cisco Packet Tracer :
Cisco Packet Tracer est un outil de simulation réseau puissant, utilisé pour l'enseignement et l'apprentissage des concepts complexes de mise en réseau. Il permet aux utilisateurs de concevoir, configurer et dépanner des architectures réseau sans avoir besoin d'équipements physiques. Cet outil peut simuler une large gamme de périphériques réseau, tels que des routeurs, des commutateurs, des serveurs et des terminaux, et permet aux utilisateurs de créer, configurer et connecter des topologies réseau dans un environnement virtuel.

### Quelques notions fondamentales:

#### Modele OSI (Open System Interconnect)
Définir des protocoles et procédures normalisés qui autorisent des systèmes hétérogènes (dits ouverts) à
s'interconnecter et à échanger des informations.s'intéresse au processus de communication entre systèmes informatiques.
Les 7 couches du modèle OSI:
1. Physique
2. Liaison
3. Reseau
4. Transport
5. Session
6. Presentation
7. Application

* OSI Couche 1 = Physique
La couche physique traite des caractérisques physiques (électriques,
électroniques, etc.) des média de transmission aussi bien au niveau des
LAN que des WAN.
Exemples d’équipements de couche 1: Hub, Répeteur, Convertisseur de Media, UTP, fible optique connector.

* OSI Couche 2 = Liaison de données
Définit le format des données qui seront envoyées sur le câble (trames)
Définit la topologie des câbles (étoile, bus, anneau)
Etudie la manière d’accéder au support (jeton, aléatoire, timeslot, plus
fort…)
Exemples d’équipements de couche 2: Switch, Pont, Carte reseau, Adresses MAC Ethernet

* OSI Couche 3 = Réseau
En charge de l’adressage logique et de l’acheminement des données:
(ex: postale, téléphone, IP)
En charge de la transmission des données d’un réseau un autre
(routeur)
En charge de trouver le meilleur chemin entre A et B: Comparable aux
services de la poste
Format universel du paquet de données(datagramme)
Exemples d’équipements de couche 3: Routeur, Adresses IPv4, IPv6 

* OSI Couche 4 = Transport
Gère la circulation des données de bout en bout
Identifie les processus terminaux
Un autre niveau d’adressage (numéro de port)
Peut fournir un transport stable
Flux de taille illimitée
Correction d’erreur et retransmission
Livraison dans le bon ordre
Contrôle de flux
découpage/réassemble les données à transmettre
Exemples d’équipements de couche 4: fireware, Numéros de port TCP et UDP

* OSI Couche 5 = Session
Ouvre, ferme les sessions de dialogue
Rétablit la connexion de transport si elle échoue
Multiplexer les données sur plusieurs connexions de transport
Eventuellement authentifie les membres du dialogue
Syncrhronise le dialogue (alternatif, simultané, tour de rôle)

* OSI Couche 6 = présentation
Réorganise les données: Traduction d’un jeu de caractères
Définit le format des données (texte, image, son, nombres)
Réalise aussi le chiffrement et/ou la compression des données
(optionnel)
Permet la conversion (traduction) de fichiers

*OSI Couche 7 = Application
Ce sont les programmes de l’utilisateur
Exemple: Navigateur Internet, Mail, FTP, Telnet, SSH, DHCP, DNS
Fournit des accès réseaux aux programmes classiques


#### L adresse IP 
Les adresses IP se sont des identifiants unique a des appareils sur un reseaux, permettant d'acheminer des paquets d'informations vers leur destination et d'assurer une communication fiable. 
Les adresses IP sont base sur un systeme de notation binaire ou decimale.
Une adresse IP (IPv4) est composée de 32 bits, divisés en quatre octets, représentant chacun une valeur de 0 à 255.
Format : Les adresses IP sont écrites en « notation décimale pointée », avec quatre sections séparées par des points (par exemple, \(192.168.1.1\)).

#### Un cable RJ-45
C est un cable ethernet utilise pour transmettre des donnees sur des reseaux locaux.
- les types de cables
1. cable droit: utiliser pour raccorder un PC a une prise.
2. cable croise: utiliser pour raccorder 2 PC directement ou en general 2 equipements de meme nature.
3. cable console: comme un cable droit mais inverse.

#### switch
Relier plusieurs appareils comme un hub, mais avec intelligence.
Le switch lit les adresses MAC et envoie les données uniquement à la bonne machine.
✔ Avantages :

- Pas de collisions
- Réseau plus rapide
- Plus sécurisé
- Plus utilisé aujourd’hui

#### hub
Un hub est un appareil réseau très simple qui sert à relier plusieurs appareils entre eux dans un réseau local (LAN).
une multiprise réseau.
Il reçoit les données depuis un port et les renvoie à tous les autres ports, sans réfléchir.

#### Routeur
Le routeur est un appareil reseau qui permet d interconnecter plusieur reseaux differents.
Le routeur lit les adresses IP, choisit la bonne route dans sa table de routage, et transporte les données d’un réseau à l’autre.
Exemple:
ton réseau local → Internet
réseau 192.168.1.0/24 → réseau 192.168.2.0/24

#### La distinction entre le commutateur(switch) et le routeur
Un commutateur connecte des appareils dans un même réseau alors qu un routeur connecter plusieurs réseaux différents.
Un commutateur utilise une adresse MAC et envoie les données uniquement à la bonne machine alors qu un routeur utilse une adresse IP.
Un commutateur envoie les données à un appareil précis alors qu un routeur envoie les données à un reseau precis.

#### La passerelle par défaut
La passerelle par defaut c est la porte de sorti ou d entre d un packet(message). 

#### La distinction entre le switch et le hub
Le switch envoie seulement au bon destinataire alors que le hub répète les données à tout le monde.
Contrairement au switch, le hub ne sait pas :

- lire les adresses MAC
- diriger le trafic vers le bon appareil
- filtrer les données

#### Un serveur et son role 
Un ordinateur ou un système informatique puissant qui fournit des ressources, des données ou des services à d'autres ordinateurs, appelés « clients », via un réseau.
role: il reçoit une requête → il répond en envoyant un résultat.

#### DHCP 
Distribution automatique des adresses IP, une gateway, un DNS aux machines.

#### DNS (Domain Name System) et son rôle dans la communication réseau
Le service DNS permet de faire la correspondance entre des noms de machine et des adresses IPs.
Le service DNS permet aux utilisateurs d'accéder à des sites Web, d'envoyer des e-mails et d'effectuer d'autres
activités Internet en dirigeant les requêtes vers les emplacements appropriés,  de faciliter l'accès aux sites web et services en ligne grâce à des noms plus faciles à retenir que des adresses IP.

Quels sont les différents types d'enregistrements DNS et à quoi servent-ils ?
* Types d'enregistrements DNS courants
- Enregistrement A : Lie un nom de domaine à une adresse IPv4.
- Enregistrement AAAA : Lie un nom de domaine à une adresse IPv6.
- Enregistrement CNAME : Crée un alias (nom canonique) pour un autre nom de domaine, ce qui permet de pointer plusieurs domaines vers un seul serveur.
- Enregistrement MX : Spécifie le ou les serveurs de messagerie responsables de la réception des e-mails pour un domaine.
- Enregistrement TXT : Stocke des informations textuelles pour les domaines. Il est utilisé pour des vérifications de domaine (comme le propriétaire) et pour des politiques de sécurité comme SPF, DKIM et DMARC.
- Enregistrement NS : Indique les serveurs de noms faisant autorité pour un domaine.
- Enregistrement SRV : Spécifie l'emplacement d'un service spécifique (par exemple, pour la messagerie instantanée ou VoIP).
- Enregistrement SOA : Contient des informations administratives sur la zone DNS, comme le contact du responsable.
- Enregistrement PTR : Utilisé pour les recherches DNS inversées (qui permettent de trouver un nom de domaine à partir d'une adresse IP). 

#### L'objectif HTTP(Hypertext Transfer Protocol) et le mode d'utilisation des réseaux
L HTTP est un protocole de communication fondamental du WWW(World Wide Web), permet l echange des donnees entre un client(navigateur) et un serveur web en utilisant des requêtes et des réponses pour transférer des ressources comme des pages web, des images ou des fichiers.

#### HTTPS et HTTP
Le protocole HTTP transmet des données non chiffrées, ce qui signifie que les informations envoyées depuis un navigateur peuvent être interceptées et lues par des tiers. Ce processus n'étant pas idéal, il a été étendu au protocole HTTPS pour ajouter une couche de sécurité supplémentaire aux communications. Le protocole HTTPS associe les requêtes et les réponses HTTP aux technologies SSL et TLS.

Les sites Web HTTPS doivent obtenir un certificat SSL/TLS auprès d'une autorité de certification (CA) indépendante. Ces sites Web partagent le certificat avec le navigateur avant d'échanger des données pour établir la confiance. Le certificat SSL contient également des informations cryptographiques, qui permettent au serveur et aux navigateurs Web d'échanger des données chiffrées ou brouillées. 

#### FTP (File Transfer Protocol)
C est un protocole réseau standard utilisé pour transférer des fichiers entre ordinateurs, généralement entre un client et un serveur.

Le protocole FTP a la particularité d'ouvrir deux connexions TCP différentes entre le client et le serveur. Une connexion est chargée de transmettre les informations de contrôle entre le client et le serveur, tandis que l'autre est utilisée pour le transfert de fichiers proprement dit.

#### TCP et UDP
Ce sont des protocoles de transport permetant d acheminer les donnees sur internet mais de maniere differente.
TCP (orienté connexion, fiable, circuit virtuel, lourd).
UDP (sans connexion, non fiable, léger et rapide).

#### Definition d un PORT
Un port est une porte logique utilisée pour identifier un service ou une application sur un ordinateur lorsqu’il communique sur un réseau.
Les ports servent à séparer ces services.
Un port :
✔ est un numéro
✔ identifie un service ou une application
✔ permet à une machine de gérer plusieurs communications ou service à la fois
✔ fonctionne au niveau du transport (TCP/UDP)

Les ports sont utilisés au niveau de la couche de transport pour identifier des applications spécifiques, tandis que les protocoles sont attribués à différentes couches du modèle OSI (ou à leurs équivalents dans le modèle TCP/IP) pour gérer des fonctions de communication distinctes. 
Par exemple, le protocole HTTP (couche Application) utilise TCP (couche Transport) via le port 80 pour la communication web. 
Protocole et couche OSI associés
- Protocole    Couche OSI   Port TCP/UDP (si applicable)             Fonction principale  
- HTTP         Application   (80) (port par défaut)                   Transfert de pages web
- FTP          Application   (21) (commande) et (20)(données)         Transfert de fichiers
- SMTP         Application   (25)                                     Envoi d'e-mails
- DNS          Application   (53)                                     Résolution de noms de domaine en adresses IP
- DHCP         Application   (67) et (68)                             Attribution automatique d'adresses IP 
- TCP          Transport    (Utilise les ports de l'application)      Connexion fiable et orientée flux de donnée
- UDP          Transport    (Utilise les ports de l'application)      Connexion non fiable (rapide et légère)
- IP           Réseau       (Sans port spécifique)                    Routage des paquets entre les réseaux
- ARP          Réseau / Liaison de données(Sans port spécifique)      Résolution d'adresses IP en adresses physiques (MAC)
- Ethernet    Liaison de données / Physique(Sans port spécifique)     Protocoles de communication sur un réseau local

#### La table de routage 
La table de routage est un élément essentiel dans tout appareil réseau (PC, routeur, serveur).
Elle contient les chemins que la machine doit utiliser pour atteindre chaque réseau.

La table de routage est une liste de routes qui indique :

* quel réseau est accessible
* via quelle interface
* via quelle passerelle
* avec quel chemin prioritaire (métrique)
Elle permet à une machine de savoir :

* comment atteindre un autre réseau,
* si le paquet reste dans le même réseau,
* ou s’il doit passer par un routeur.
* Sans table de routage → aucune communication entre réseaux.



 