# Automate qui fait le café

DEBUT
SI (pas de cafetière OU de tasse)
    FIN

SINON
    - ouvrir le panier de la cafétière
        SI (filtre usé)
            Jeter le vieux filtre à la poubelle

    - prendre un filtre
        SI (pas de filtre)
            FIN
        SINON   
            mettre le filtre dans le panier

    - prendre le café
        SI (pas de café)
            FIN
        SINON
            mettre le café dans le filtre
    - fermé le panier
    - ranger le café

    - prendre la verseuse
        SI (pas de verseuse)
            FIN
        SINON
            remplir la verseuse d'eau
                SI (pas d'eau)
                    FIN
                SINON
                    remplir le réservoir avec l'eau contenu dans la verseuse
                    replacer la verseuse

    - appuyer sur le bouton de la cafétière
        SI (pas de courant électrique)
            FIN
        SINON
            patienter jusqu'à ce que toute l'eau soit passée
    
    - prendre la verseuse pleine de café
    - remplir la tasse de café
    - remettre la verseuse en place
   
    - prendre la tasse pleine de café
    - aller jusqu'au client
        SI (client absent ET pas de bureau)
            - attendre 5 min
                SI (retour client)
                    - donner café
                    FIN
                SINON 
                    - aller vers un évier
                    - jeter le café dans l'évier
                    - laver la tasse
                    - ranger la tasse à sa place
        SI (client absent ET un bureau)
            - poser tasse sur le bureau
            FIN

        SINON 
            -  donner café
            FIN

FIN