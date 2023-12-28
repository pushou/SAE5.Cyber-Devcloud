# SAE 5 Cyber et Devcloud

## Objet de la SAE

Vous devez créer un environnement d’entraînement pour les équipes "blue team et red team" de votre entreprise.
Votre équipe sera constituée de deux membres de l'équipe Cloud et de deux membres de l'équipe Cyber.
Vous devrez mettre en œuvre un environnement technique permettant de simuler un environnement de production Windows.
Cet environnement sera basé sur le projet GOAD d'Orange Cyberdéfense qui permet de déployer un Active Directory vulnérable. 
voir https://github.com/Orange-Cyberdefense/GOAD


Dans cet environnement, vous aurez à mettre en œuvre des outils de détection (SIEM-IDS-HONEYPOT)  et un plan de test d'intrusion sur l'ensemble de l'environnement. Dans un premier temps vous mettrez en oeuvre des outils comme **blooddHound** et **Sharphound** pour cartographier AD sous forme de graphe et trouver des chemins d'attaques. 

L'**audit** et **Sysmon** devront être activés sur les machines Windows. Les Logs seront remontées sur un serveur OPENWEC. Des notes d'installation sont disponibles pour vous aider à le mettre en oeuvre.

Vous utiliserez des "sigma rules" pour detecter les attaques sur les logs EVTX.
Un IDS Suricata sera déployé aussi à l'endroit le mieux adapté.

A chaque test, vous associerez les alertes générées par le SIEM et vous analyserez les résultats. Vous utiliserez au moins deux SIEM et des outils portables comme Chainsaw et Hayabusa. Le déploiement des agents devra être automatisé.
Votre environnement sera protégé par un pare-feu virtuel ou physique Stormshield.

Cet environnement sera déployé sur une plateforme sur Virtual Box et sur Proxmox. Vous devez mener l'installation en parallèle sur les deux plateformes. 

La répartition du travail eu sein de l'équipe est libre, mais doit être planifiée et quantifiée au travers d'un suivi type Jira/gitub en mode Kanban.
Votre responsable doit pouvoir suivre l'avancement de votre projet et faire un bilan personnel des tâches réalisées sous forme de graphique par chaque membre de l'équipe à la fin du projet.

Vous serez aidé par trois conseillers qui vous guideront lors de la mise en  œuvre de votre projet quand ils seront présents. Ces experts étant facturés à l'heure, vous devrez soigneusement réfléchir à la manière de les consulter (préparez vos questions, soyez précis dans vos demandes, etc...).
Il est impératif de faire valider votre travail par les experts qui donneront une appréciation de votre niveau de compétence sur les aspects techniques et méthodologiques.

## Technologie
- Votre infrastructure contiendra un serveur de logs (OpenWEC)
  (voir https://www.sstic.org/2023/presentation/openwec/) réceptacle des logs de vos serveurs windows.
  


## Livrables attendus

- Le plan de test d'intrusion.
- Bilan des tâches réalisées par chaque membre de l'équipe et temps passé.
- Schéma réseaux.
- Tableau de test d'intrusions et analyse des résultats correspondants sur les SIEM. Le critère de furtivité sera apprécié dans vos résultats.
- Liste des matériels utilisés par votre team ce qui permettra de retrouver sur quel matériel vous avez travaillé. L'ensemble des serveurs ne sera pas disponible les six derniers serveurs sont réservés pour une autre expérimentation (ressource Cloud sur deux journées).
- 
En annexe:

- Dépôts Git pour la partie automatisation et déploiement des agents.
- Bilan des questions posées aux experts et réponses apportées.
- Traces des installations et des configurations réalisées.

Au final l'ensemble des matériels devra être ré-initialisé avant la fin de la SAE. Un manquement à cette règle entraînera une pénalité sur l'appréciation de vos compétences.
