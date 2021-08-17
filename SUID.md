
# Definition du SUID

Ce droit s'applique aux fichiers exécutables, il permet d'allouer temporairement à un utilisateur les droits du propriétaire du fichier, durant son exécution. En effet, lorsqu'un programme est exécuté par un utilisateur, les tâches qu'il accomplira seront restreintes par ses propres droits, qui s'appliquent donc au programme. Lorsque le droit SUID est appliqué à un exécutable et qu'un utilisateur quelconque l'exécute, le programme détiendra alors les droits du propriétaire du fichier durant son exécution. Bien sûr, un utilisateur ne peut jouir du droit SUID que s'il détient par ailleurs les droits d'exécution du programme. Ce droit est utilisé lorsqu'une tâche, bien que légitime pour un utilisateur classique, nécessite des droits supplémentaires (généralement ceux de root). Il est donc à utiliser avec précaution. Pour des partitions supplémentaires, il faut activer le bit suid pour pouvoir l'utiliser en le spécifiant dans les options des partitions concernés dans le fichier fstab.

## Comment reconnaitre 

Son flag est la lettre s ou S qui vient remplacer le x du propriétaire. La majuscule ou la minuscule du 's' permet de connaitre l'état du flag x (droit d'exécution du propriétaire) qui est donc masqué par le droit SUID 's' ou 'S': C'est un s si le droit d'exécution du propriétaire est présent, ou un S sinon. Il se place donc comme ceci :

* ---s------  ou  ---S------

Un fichier avec les droits

* -rwxr-xr-x

auquel on ajoute le droit SUID aura donc la notation

* -rwsr-xr-x
