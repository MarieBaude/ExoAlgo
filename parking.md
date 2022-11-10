FONCTION payerMachine
    - entré le ticket dans la machine
    - suivre les instructions de payment
    SI (retour ticket)
        - récupéré son ticket payé 

FONCTION allerSortie
    - aller jusqu'à la voiture
    - conduire la voiture jusqu'à la porte de sortie


DEBUT

    - entrer dans le parking

    # borne dans le parking
    SI (paiment à une borne)
        - se rendre à la borne
            SI (ticket)
                - f : payerMachine
            
            SINON
                - prendre contact via le bouton d'interphone
                - communiquer votre plaque d'immatriculation
                - génération d'un nouveau ticket
                - suivre les instructions de payment
                - récupéré son ticket payé
    
        - f : allerSortie

    
    SINON
        - f : allerSortie
        
        # badge
        SI (badge)
            - présenter le badge

        # borne à la sortie
        SINON
            - f : payerMachine

    
    - ouverture de la barre de sécurité
    - sortie du parking

    SINON
        - voiture bloqué

FIN

Problème possible :
- panne électrique -> ouverture de la barrière manuel possible
- client pas d'argent ->
- barrière bloquer -> envoie de message d'erreur au gardien, ouverture de la barrière manuel possible
- 