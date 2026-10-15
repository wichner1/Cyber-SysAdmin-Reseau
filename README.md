# Cyber-SysAdmin-Reseau
Portfolio de démonstration de LABs mis en œuvre, servant à simuler des scénarios d'entreprise concrets en administration réseau, systèmes et cybersécurité. Avec Systeme Hybride  AD synchro avec Entra ID via Azure Adconnect (ADDConnect)

Architechture Reseau mise en place 
j'utilise un 10.0.0.0 /8 comme Adresse global avec objectif de definir une architecture qui sera sur plisieurs site avec le 2eme octet comme les Vlan et  d'utiliser le 3ème octet pour faire correspondre a chaque site   pour une convention simple, lisible et très efficace pour la gestion quotidienne 

Comme mon réseau de base est 10.0.0.0, j'ai structuré cela en utilisant un masque de sous-réseau en /24 (masque
255.255.255.0) pour chaque VLAN. Ce qui me donne 254 adresses IP utilisables par  Vlan , ce qui est largement suffisant
pour les des départements tout en isolant parfaitement le trafic.

Voici en exemple le cas du departement TI la proposition de découpage propre et optimisée pour votre architecture

VLAN 20  TI (Informatique)  site 100 : 10.20.100.1 à 10.20.100.254  255.255.255.0 (/24)  

se sera la meme chose avec mes autres VLANs

vlan30 Finance & Comptabilité  10.10.20.1 à 10.10.20.254  255.255.255.0 (/24)  10.10.20.1 ou .254

vlan40 Logistique

vlan50 Ressources Humaines

vlan60 Ventes & Marketing / Opérations

vlan70 Bureautique

vlan90 Wifi

VLAN 10 – Gestion

les serveurs qui sont utilisees :
Active directory (En Premise )
( Fichier, Azure Adconnect, deux autre DC, Serveur de Sauvgarde,Gestionnaire de mot de passe ( Linux acces interface Web) 
<img width="1408" height="768" alt="Gemini_Generated_Image_r0ckavr0ckavr0ck" src="https://github.com/user-attachments/assets/01533381-71fc-4b3e-8454-3f8a910a66d8" />
