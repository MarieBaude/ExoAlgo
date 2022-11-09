# Automate qui fait le café

DEBUT
SI (pas de cafetière complète OU de tasse OU de café OU de filtre OU d'eau OU d'électricité)
    FIN

SINON
    - ouvrir le panier de la cafétière
        SI (filtre usé)
            Jeter le vieux filtre à la poubelle
        
    - prendre un filtre 
    - mettre le filtre dans le panier
    - prendre le café
    - mettre le café dans le filtre
    - fermer le panier
    - ranger le café

    - prendre la verseuse
    - remplir la verseuse d'eau
    - remplir le réservoir avec l'eau contenu dans la verseuse
    - replacer la verseuse

    - appuyer sur le bouton de la cafétière
    - patienter jusqu'à ce que toute l'eau soit passée
    
    - prendre la verseuse pleine de café
    - remplir la tasse de café
    - remettre la verseuse en place
   
    - prendre la tasse pleine de café
    - aller jusqu'au client
        SI (bureau)
            - poser le café sur le bureau
        SINON
            - donner le café au client      

FIN