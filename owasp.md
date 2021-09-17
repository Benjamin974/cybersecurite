## Qu’est-ce que l’OWASP ?

Le projet de sécurité des applications web ouvertes tient une liste régulièrement mise à jour des préoccupations les plus urgentes en matière de sécurité des applications web.

## Définition de l’OWASP ?

L’Open Web Application Security Project, ou OWASP, est une organisation internationale à but non lucratif qui se consacre à la sécurité des applications web. L’un des principes fondamentaux de l’OWASP est que tous ses documents soient disponibles gratuitement et facilement accessibles sur son site web, ce qui permet à chacun d’améliorer la sécurité de ses propres applications web. Le matériel qu’ils proposent comprend de la documentation, des outils, des vidéos et des forums. Leur projet le plus connu est peut-être le Top 10 de l’OWASP.

## Top 10 des l’OWASP ?

Le Top 10 de l’OWASP est un rapport régulièrement mis à jour qui expose les préoccupations en matière de sécurité des applications web, en se concentrant sur les 10 risques les plus critiques. Le rapport est élaboré par une équipe d’experts en sécurité du monde entier. L’OWASP qualifie le Top 10 de « document de sensibilisation » et recommande à toutes les entreprises d’intégrer le rapport dans leurs processus afin de minimiser et/ou d’atténuer les risques de sécurité.

## mise a jour 2021 

A01:2021-Broken Access Control passe de la cinquième position ; 94% des applications ont été testées pour une forme de contrôle d'accès cassé. Les 34 CWE mappés à Broken Access Control ont eu plus d'occurrences dans les applications que toute autre catégorie.

A02:2021-Les échecs cryptographiques passent d'une position à la 2ème position, anciennement connue sous le nom d' exposition de données sensibles, qui était un symptôme général plutôt qu'une cause première. L'accent renouvelé ici est mis sur les défaillances liées à la cryptographie qui conduisent souvent à l'exposition de données sensibles ou à la compromission du système.

A03:2021-Injection glisse vers la troisième position. 94% des applications ont été testées pour une certaine forme d'injection, et les 33 CWE mappés dans cette catégorie ont le deuxième plus grand nombre d'occurrences dans les applications. Le Cross-site Scripting fait désormais partie de cette catégorie dans cette édition.

A04:2021-Insecure Design est une nouvelle catégorie pour 2021, avec un accent sur les risques liés aux défauts de conception. Si nous voulons vraiment « aller à gauche » en tant qu'industrie, cela nécessite une plus grande utilisation de la modélisation des menaces, des modèles et principes de conception sécurisés et des architectures de référence.

A05:2021-Security Misconfiguration passe de #6 dans l'édition précédente ; 90% des applications ont été testées pour une certaine forme de mauvaise configuration. Avec de plus en plus d'évolutions vers des logiciels hautement configurables, il n'est pas surprenant de voir cette catégorie progresser. L'ancienne catégorie des entités externes XML (XXE) fait désormais partie de cette catégorie.

A06:2021-Vulnerable and Outdated Components était auparavant intitulé Using Components with Known Vulnerabilities et est n°2 dans l'enquête du secteur, mais disposait également de suffisamment de données pour figurer dans le Top 10 via l'analyse des données. Cette catégorie passe de la 9e place en 2017 et est un problème connu que nous avons du mal à tester et à évaluer les risques. C'est la seule catégorie à ne pas avoir de CVE mappés sur les CWE inclus, donc un exploit par défaut et des poids d'impact de 5,0 sont pris en compte dans leurs scores.

A07:2021-Identification and Authentication Failures était auparavant Broken Authentication et glisse vers le bas de la deuxième position, et inclut désormais les CWE qui sont davantage liés aux échecs d'identification. Cette catégorie fait toujours partie intégrante du Top 10, mais la disponibilité accrue de référentiels standardisés semble y aider.

A08 : 2021-Défaillances d'intégrité des logiciels et des données est une nouvelle catégorie pour 2021, qui se concentre sur l'élaboration d'hypothèses relatives aux mises à jour logicielles, aux données critiques et aux pipelines CI/CD sans vérifier l'intégrité. L'un des impacts pondérés les plus élevés des données CVE/CVSS mappées sur les 10 CWE de cette catégorie. La désérialisation non sécurisée de 2017 fait désormais partie de cette catégorie plus large.

A09 : 2021 - La journalisation de la sécurité et les échecs de surveillance étaient auparavant la journalisation et la surveillance insuffisantes . Cette catégorie est étendue pour inclure plus de types de défaillances, est difficile à tester et n'est pas bien représentée dans les données CVE/CVSS. Cependant, les défaillances de cette catégorie peuvent avoir un impact direct sur la visibilité, les alertes d'incident et la criminalistique.

A10:2021-Server-Side Request Forgery est ajouté à partir de l'enquête de l'industrie (#1). Les données montrent un taux d'incidence relativement faible avec une couverture de test supérieure à la moyenne, ainsi que des notes supérieures à la moyenne pour le potentiel d'exploitation et d'impact. Cette catégorie représente le scénario où les professionnels de l'industrie nous disent que c'est important, même si cela n'est pas illustré dans les données pour le moment.