# Parking
FONCTION
``` 
FONCTION payerMachine
    - entré le ticket dans la machine
    - suivre les instructions de paiment
    SI (retour ticket)
        - récupéré son ticket payé 

FONCTION allerSortie
    - aller jusqu'à la voiture
    - conduire la voiture jusqu'à la porte de sortie

FONCTION ouvertureManuel
    - responsable se déplace physique jusqu'à la barre
    - ouverte de la barre manuellement 
```


DEBUT

    - entrer dans le parking

    SI (paiment à une borne)
        - se rendre à la borne
        SI (ticket)
            - f : payerMachine
        
        SINON
            - prendre contact via le bouton d'interphone
            - communiquer la plaque d'immatriculation
            - génération d'un nouveau ticket
            - suivre les instructions de paiment
            - récupéré son ticket payé
    
        - f : allerSortie
        - présentation ticket payé
    
    SINON
        - f : allerSortie
        
        SI (badge)
            - présenter le badge

        SINON
            - f : payerMachine

    - ouverture de la barre de sécurité

    SI (barrière en panne)
        - envoie d'un message d'erreur
        - f : ouvertureManuel
    
    SI (panne de courant)
        - f : ouvertureManuel

    - sortie du parking

FIN
