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

    SI (paiment à une borne)
        - se rendre à la borne
            SI (ticket)
                - payerMachine
            
            SINON
                - prendre contact via le bouton d'interphone
                - communiquer votre plaque d'immatriculation
                - génération d'un nouveau ticket
                - suivre les instructions de payment
                - récupéré son ticket payé
    
        - allerSortie

    
    SINON
        - allerSortie
        
        SI (badge)
            - présenter le badge

        SINON
            - payerMachine

    
    - ouverture de la barre de sécurité
    - sortie du parking

FIN