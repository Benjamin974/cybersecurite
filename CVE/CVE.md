# Definition CVE

L'acronyme CVE, pour Common Vulnerabilities and Exposures en anglais, désigne une liste publique de failles de sécurité informatique. Lorsque l'on parle d'une CVE, on fait généralement référence à une faille de sécurité à laquelle un identifiant CVE a été attribué.

Les avis de sécurité publiés par les fournisseurs et chercheurs mentionnent presque toujours au moins un identifiant CVE. Les CVE aident les professionnels à coordonner leurs efforts visant à hiérarchiser et résoudre les vulnérabilités, et ainsi renforcer la sécurité des systèmes informatiques.

## Critères d'attribution d'un identifiant CVE

Les identifiants CVE sont attribués aux failles qui répondent à un ensemble de critères spécifiques :

1. Possibilité de correction indépendante
Chaque faille doit pouvoir être corrigée indépendamment de tout autre bogue.

2. Reconnaissance par le fournisseur concerné OU documentation
L'éditeur de logiciel ou le fabricant de matériel doit reconnaître le bogue et son effet négatif sur la sécurité. Ou, la personne qui a signalé le bogue doit partager un rapport de vulnérabilité qui permet de démontrer que le bogue a un effet négatif ET qu'il enfreint la politique de sécurité du système touché.

3. Impact sur un code base
Les failles qui touchent plus d'un produit doivent recevoir différents identifiants CVE. Dans le cas de bibliothèques, protocoles ou normes partagés, la faille reçoit un seul identifiant CVE uniquement s'il n'existe aucun moyen d'utiliser le code partagé sans être affecté par la vulnérabilité. Dans le cas contraire, chaque code base ou produit affecté obtient un identifiant CVE unique.

## Exemple CVE 

Telegram Web K Alpha 0.6.1 autorise XSS via un nom de document.

### Scores CVSS et types de vulnérabilité

- Score CVSS:	4.3
- Impact sur la confidentialité :	Aucun (Il n'y a aucun impact sur la confidentialité du système.)
- Impact sur l'intégrité:	Partielle (la modification de certains fichiers système ou informations est possible, mais l'attaquant n'a pas le contrôle sur ce qui peut être modifié, ou la portée de ce que l'attaquant peut affecter est limitée.)
- Impact sur la disponibilité:	Aucun (Il n'y a aucun impact sur la disponibilité du système.)
- Complexité d'accès:	Moyen (Les conditions d'accès sont quelque peu spécialisées. Certaines conditions préalables doivent être satisfaites pour être exploitées)
- Authentification:	Non requis (L'authentification n'est pas requise pour exploiter la vulnérabilité.)
- Accès obtenu:	Rien

## Source 

https://www.redhat.com/fr/topics/security/what-is-cve
https://www.cvedetails.com/vulnerability-list/year-2021/month-7/July.html