# FirstCobolProject

Contexte et contenu :

A la fin d'une formation au language Cobol et le système d'exploitation z/OS, on a réalisé un projet d'application. Un programme pour gérer le stock de marchandises en fonction des commandes clients d'une entreprise de grande distribution avant et après livraison.

On avait à disposition des tables de base de données Db2, voir la représentation de la base de données à l'aide de la méthode Merise (MODELE). Puis les codes pour la création des différentes tables et de l'insertion des éléments de chaque table sont dans le répertoire (dans DCLGEN et SPUFI)

On a développé 4 programmes qui ont chacun un rôle :  

   -STOCK retranscrit dans un fichier les différents produits et leur quantité
  
   -CALCUL REAPPRO trie les produits à réapprovisionner et ceux à quantité suffisante selon les commandes clients à effectuer dans deux fichiers différents
  
   -MAJ APPRO calcule la quantité de produit à réapprovisionner pour chaque produit et met à jour les tables APPRO et PRODUITS avec les nouvelles quantités
  
   -LIVRAISON met à jour les stocks de la table produits selon les livraisons réalisées et changement du statut des commandes
  
  Pour une meilleure compréhension du rôle de chaque programme et de leur écriture, leur diagramme et code source sont aussi dans des dossiers.
  Le répertoire comprend aussi le JCL (CNTL) du projet.
