# FirstCobolProject

Contexte

Au terme d'une formation en COBOL, mes camarades et moi-même avons réalisé un projet de trois jours permettant de mettre en lien différentes tables et bases de données DB2 modélisant les commandes et réapprovisionnements de produits d'un site de grande distribution. Cet exécutable JCL mettait en lien différents programmes avec entrées et sorties de fichiers ainsi que des requêtes SQL donnant accès à des tables de bases de données DB2 permettant de mettre à jour les commandes des clients, le stock des produits ainsi que les quantités de réapprovisionnement du site en question.

Ainsi parmi les programmes que nous avons créés et que l'on peut retrouver dans le dossier SOURCE, on peut distinguer :

   -STOCK qui retranscrit dans un fichier les différents produits et leur quantité
  
   -CALCUL REAPPRO qui trie les produits à réapprovisionner et ceux à quantité suffisante selon les commandes clients à effectuer dans deux fichiers différents
  
   -MAJ APPRO qui calcule la quantité de produit à réapprovisionner pour chaque produit et met à jour les tables APPRO et PRODUITS avec les nouvelles quantités
  
   -LIVRAISON qui met à jour les stocks de la table produits selon les livraisons réalisées et changement du statut des commandes

Le dossier contient également les codes d'éxecution JCL (CNTL) ainsi que les codes des tables DB2 (SPUFI, DCLGEN).

Pour une meileure compréhension du programme, vous pouvez vous référer au dossier MODELE et DIAGRAMME qui contiennent un diagramme modélisant le programe ainsi que la représentation Merise des tables DB2 et les schémas des algorithmes de chaque programme.
  

