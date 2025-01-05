# ML-Duplicate-Ellipse

Duplicate Bug Report Detection
TP initialement créé par Irving Muller Rodrigues pour le cours de fouilles de données de Montréal.

Date de remise: 08/11/2024

1 - Présentation
En raison de la complexité des systèmes logiciels, les bugs logiciels sont répandus. Les entreprises, en particulier les grandes, utilisent généralement un système de suivi des bugs (BTS) pour gérer et suivre les enregistrements des bugs. Outre les développeurs et les testeurs, de nombreux projets, principalement des projets open source, permettent aux utilisateurs de signaler de nouveaux bugs dans leur BTS. Pour ce faire, les utilisateurs doivent remplir un formulaire avec plusieurs champs. Un sous-ensemble important de ces champs fournissent des données catégorielles et n'acceptent que les valeurs qui vont d'une liste fixe d'options (par exemple, composant, version et produit du système). Deux autres domaines importants sont le résumé et la description. Les utilisateurs sont libres d'écrire quoi que ce soit dans les deux champs et la seule contrainte est que le résumé a un nombre maximum de caractères. La soumission d'un formulaire crée une page, appelée rapport de bug ou rapport de problème, qui contient toutes les informations sur un bug.

Le manque de communication et de synchronisation font que les utilisateurs peuvent ne pas savoir qu'un bug spécifique a déjà été soumis et le signaler à nouveau. Identifier les rapports de bugs en double est une tâche importante dans les BTS et c'est le sujet de ce TP. Notre objectif est de développer un système qui prédit si une paire de rapports de bug soumis sont dupliqué ou non. Ce système pourra être utilisé pour identifier automatiquement les rapports dupliqués.

(fichier json disponible par dm)
