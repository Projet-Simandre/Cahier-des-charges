Esp32 * 4 (3 modules + 1 maitre)
connection par wifi
3D des chaques idées
cable M/F - F/F - M/M
Capteur température / GPS / humidite

ESP en C++ -> envoie de la donnée sur un serveur -> envoie de la donnee sous un .txt -> lecture du .txt en php sur un site web (recuperation de la derniere ligne)

stabiliser le site pour eviter que les données sur le site chagent trop souvent (donnee recu toutes les 15min)
site web avec historique

securisation de la selection des données via le wifi en mettant un mot clé au debut de chaque nom 
exemple : Hexagone - //// le mot "Hexagone -" est le mot clé et est accepte par le wifi tout en excluant les autres

le fichier texte doit contenir 6 mois de donnee - trier l'ordre de recu par numero (1.// pour un capteur  2.// pour un autre  ...) - 

besoin : 
    capter les données
    transmettre les donnees au serveur en limitant la perte
    affichage des donnees sur un site web

° module wifi / envoyer la donnee
° recevoir les donnees des capteurs 
° lire la donnee (PHP), affiche HTML
° capteur humidité / temperateur / GPS 

but :
    afficher les donnees meteo sur une interface web a un emplacement spécifier


ajout d'un serveur de backup (au cas ou ESP maitre crash)
Ajout d'un protocole HELLO entre les ESP pour assurer la connection entre l'ESP maitre et les ESP des composants
si ESP maitre crash alors les ESP composant envoient directement l'info au serveur


Pour eviter la perte de la donnée en cas de crash d'un composant 
ajouter un chiffre correspondant à chaque composant dans le traitement de donnee et si un composant ne repond pas le remettre a 0
exemple (1./// , 2./// , 3.///) si le composant 3 crash alors on aura : 1./// , 2./// , 3.000
