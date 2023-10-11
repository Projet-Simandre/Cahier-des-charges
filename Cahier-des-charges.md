Esp32 * 4
connection par wifi
3D des chaques idées
cable M/F - F/F - M/M
Capteur température / GPS

Carte en C++ -> envoie de la donnée en .txt -> lecture de la donnée en python sur un site web (recuperation de la derniere ligne)
fichier bash python pour le faire boucler

stabiliser le site pour eviter que les données sur le site chagent trop souvent 
site web avec historique

securisation du wifi en mettant un mot clé au debut de chaque nom 
exemple - Hexagone - //// le mot "Hexagone -" est le mot clé et est accepte par le wifi tout en excluant les autres

limiter le nombre de ligne sur le fichier texte - maximum 96 lignes (1 donnee toutes les 15min pour 1 journee)
a la 97e lignes, on sup la 1ere ligne (la plus ancienne)

besoin : 
    capter les données
    transmeettre les donnees tout en limitant le nb de ligne
    affichage des donnees sur un site web

° module wifi / envoyer la donnee
° recevoir les donnees des capteurs 
° traiter, ajouter dans un fichier txt (limitation des lignes)
° lire la donnee (Python), affiche HTML
° capteur humidité / temperateur / GPS 

but :
    afficher les donnees meteo sur une interface web a un emplacement spécifier

repartition des taches 
Sirine - 
Imrane - 
Alexandre - 