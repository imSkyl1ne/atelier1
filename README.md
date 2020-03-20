# CAPTURE 1:

1/ curl http://capgchamb15.goffinet.net:8003

La commande curl effectue une requête sur le serveur, ici en protocole HTTP sur le serveur capgchamb15......... 

name: capgchamb15.goffinet.net
ipv4: 51.158.72.164

2/ Voir capture1.pcapng

3/ le port source utilisé par le client est 40024 à direction du port 8003 

4/ La commande de couche Application est GET, celle-ci est contenue dans le paquet n°14 de la capture 

5/ Le paquet qui commence la session est le paquet 11 [SYN], et le paquet qui termine la session est le paquet 22 [ACK]


# CAPTURE 2:

1/ Cette commande utilise l'outil dig, qui permet d'interroger des serveurs DNS. Ici on utilise le resolveur DNS de google. "Short -4" permet je crois de limiter l'affichage uniquement à l'adresse IPv4. Le but étant d'obtenir l'adresse IPv4 du site web "o-o.myaddr.l.google.com" à partir de son URL en interogeant un serveur DNS. 

2/ Voir capture2.pcapng

3/ 2 transactions sont générées avec cette commande, car il y a l'envoi de la requête au serveur DNS puis la réponse de celui-ci

4/ Le query posé par ces transactions est TXT (text records) 

5/ la première transaction pose la question à la machine 216.239.32.10 (serveur DNS) et dans la deuxième transaction, la réponse, est envoyée à 192.168.1.1 (machine utilisateur) 
