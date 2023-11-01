# ical
récupération de calendrier + traitement (recherche de disponibilités)

Ce projet a pour but l'utilisation du calendrier de la haure école afin de:
- récupérer le calendrier
- faire des recherches dans celui-ci
- extraire la disponibilité des classes (groupes)
- extraire la disponibilité des locaux
- construire des propositions de changement d'horaire (pas encore implémenté)
- construire des propositions d'horaire (pas encore implémenté)

Ce projet s'articule sur deux volets:
- la récupération des informations
- le traitement de ces informations

La récupération des informations se fait à l'aide de l'application "Actiona" 
qui (fonctionne sous Linux et Windows). Cette application est seulement citée 
ici (elle n'est pas traitée ou incorporée).
Seul est partagé ici le script créé sous Actiona. 
Ce script, pour fonctionner 
correctement doit être adapté à votre situation. Il a été développé avec le navigateur
Firefox, et sur une écran de résolution 2560x1080. Il en va de même pour
les images qui sont des actures d'écran réalisés dans cette résolution. Ces actptures
d'écran sont utilisées dans le script pour localiser une zone pour y 
réaliser une action.
Ces actions relèvent parfois d'actions sur un navigateur. Votre connexion pourrait
rendre les réponses de celui-ci moins rapides, auquel cas, il faudra adapter les pauses.
Ces pauses sont soit de "pauses", soit des paramètres "pause after" ou "pause before"
dans les paramètres "common" des actions dans le script.
Ce script récupère l'agenda de chaque local kdisponible pour les activités.

Le traitement des données se fait via un scrip python. Il est possible d'adapter 
celui-ci pour avoir un traitement en une fois et obtenir ce que l'on cherche. Il
est aussi possible d'importer le module "ical.py" dans un terminal. La fonction récupérant
tous les calendriers prend quelque (longues) secondes.
Une aides sur les fonctions du module peut être obtenue avec "help(ical)". Ou encore
help(<nom de la fonction>).
(Certains helpdoc sont encore en voie de finalisation.
