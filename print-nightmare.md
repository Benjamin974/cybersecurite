# Définition de print nightmare

Le nouveau CVE-2021-34527 alias "Print Nightmare" est une vulnérabilité qui affecte le service de pool d'impression, qui est activé par défaut sur la machine Windows. L'exploitation réussie de la vulnérabilité permettra effectivement à un attaquant d'exécuter des fichiers DLL sur le système cible (Exécution de code à distance) dans le contexte du service vulnérable, qui s'exécute avec les privilèges SYSTEM.

 La vulnérabilité est considérée comme dangereuse car un attaquant peut prendre le contrôle total de n'importe quel serveur Windows dans les conditions ci-dessous :

· Le service vulnérable « Print Spooler » est activé sur la machine cible. 

· Connectivité réseau à la machine cible

· Identifiants pour un compte utilisateur peu privilégié


## Comment ça marche 

Le print spooler service  a une fonction appelée RpcAddPrinterDrive, qui permet aux utilisateurs d'ajouter des pilotes à un print spooler distant ; cette activité est normale et est conçue pour permettre aux administrateurs informatiques d'installer à distance des pilotes d'imprimante dans un environnement de bureau. Cependant, en raison d'une faille dans la logique, n'importe quel utilisateur peut ajouter les pilotes sans avoir besoin de privilèges administratifs. Un attaquant peut exploiter la faille et piéger le service pour qu'il installe un pilote permettant l'exécution de commandes sur la machine cible avec les privilèges Système.

 Au moment de la rédaction, aucun correctif n'est encore disponible par fournisseur, cependant, des atténuations et des solutions de contournement ont été partagées par Microsoft via cette note de publication. 



## Comment s'en protéger

La première chose à faire est de désactiver le service File d’attente d’impression si votre ordinateur n’a pas d’imprimante. Si vous possédez une imprimante, nous vous recommandons la procédure suivante :

- Accédez à Modifier la stratégie de groupe.
- Allez ensuite dans Configuration de l’ordinateur.
- Cliquez sur Modèles d’administration.
- Sélectionnez Imprimantes.
- Maintenant, nous désactivons Autoriser le gestionnaire de travaux d’impression à accepter les connexions client.
- Et c’est tout, avec cette procédure, vous protégerez votre ordinateur de la vulnérabilité Print Nightmare.

