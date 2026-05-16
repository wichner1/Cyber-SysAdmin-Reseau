# Cyber-SysAdmin-Reseau
Portfolio de démonstration de LABs mis en œuvre, servant à simuler des scénarios d'entreprise concrets en administration réseau, systèmes et cybersécurité.

Architechture Reseau mise en place 
j'utilise un 10.10.0.0  dans le but d'utiliser le 3ème octet pour faire correspondre directement le numéro de VLAN pour une convention simple, lisible et très efficace pour la gestion quotidienne 

Comme mon réseau de base est 10.10.0.0, j'ai structuré cela en utilisant un masque de sous-réseau en /24 (masque
255.255.255.0) pour chaque VLAN. Ce qui me donne 254 adresses IP utilisables par sous-réseau, ce qui est largement suffisant
pour la majorité des départements tout en isolant parfaitement le trafic.

Voici en exemple le cas du departement TI la proposition de découpage propre et optimisée pour votre architecture

VLAN 10  TI (Informatique) 10.10.10.1 à 10.10.10.254  255.255.255.0 (/24)  10.10.10.1 ou .254

se sera la meme chose avec mes autres VLANs

vlan20 Finance & Comptabilité

vlan30 Logistique

vlan40 Ressources Humaines

vlan50 Ventes & Marketing / Opérations

vlan60 Bureautique

vlan70 Wifi

vlan90 Wifi-Guest

VLAN 100 – Gestion
<img width="1408" height="768" alt="Gemini_Generated_Image_r0ckavr0ckavr0ck" src="https://github.com/user-attachments/assets/01533381-71fc-4b3e-8454-3f8a910a66d8" />
