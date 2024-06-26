# Comment récupérer ses mots de passe ?

Ce tutoriel ne concerne que des machines ***Windows***. 

## Outils 

Le seul outil que nous allons utiliser est le Powershell. 

## Cibles

1. Notre propre machine
2. Machine distante

NB: Cette méthode peut aussi être utilisée pendant les intrusions. Mais je décline toute responsabilité en cas d'utilisation de ce tutoriel à des fins illicites.


## Etapes
1. Ouvrir le Powershell ou l'invite de commandes.
2. Taper les commande ci-dessous.
3. Exploiter les résultats selon ses besoins.

## Commandes

1. Lister tous les réseaux disponibles

        # Cette commande permet d'afficher tous les réseaux disponibles
        netsh wlan show profile
     
2. Cibler une seule et récupérer les informations importantes

        netsh wlan show profile  nom_du_wifi key=clear
