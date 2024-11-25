# SAE 5 Cyber et Devcloud

## Objet de la SAE

### objectifs
Vous devez créer un "Proof of Concept" pour les futures équipes "blue team et red team" d'une entreprise.
Votre équipe sera constituée de deux membres spécialistes de deux membres spécialiste Cyberbersécurité de votre ESN.

A cet effet vous devrez mettre en œuvre un environnement réaliste  permettant de simuler un environnement de production Windows.

La gestion de projet sera faite en mode agile. Les efforts seront quantifiés (nombre de taches par personne, nombre de jours par personne...).

Cet environnement sera basé sur le projet GOAD d'Orange Cyberdéfense qui permet de déployer un Active Directory vulnérable. 
voir https://github.com/Orange-Cyberdefense/GOAD


Dans cet environnement, vous aurez à mettre en œuvre des outils de détection (SIEM-IDS-HONEYPOT)  et un plan de test d'intrusion sur l'ensemble de l'environnement. Dans un premier temps vous mettrez en oeuvre des outils comme **blooddHound** et **Sharphound** pour cartographier AD sous forme de graphe et trouver des chemins d'attaques. 

L'**audit** et **Sysmon** devront être activés sur les machines Windows. Les Logs seront remontées sur un serveur OPENWEC. Des notes d'installation sont disponibles pour vous aider à le mettre en oeuvre.

Vous utiliserez des "sigma rules" pour détecter vos attaques sur les logs EVTX.
Un IDS Suricata sera déployé aussi à l'endroit le mieux adapté.

A chaque test, vous associerez les alertes générées par le SIEM et vous analyserez les résultats. Vous utiliserez au moins deux SIEM et des outils portables comme Chainsaw et Hayabusa. Le déploiement des agents devra être automatisé.


Cet environnement sera déployé sur une plateforme sur "Virtual Box". 


Vous serez aidé par un ingénieur senior qui vous guidera lors de la mise en  œuvre de votre projet quand il sera présent. Cet expert étant facturé à l'heure, vous devrez soigneusement réfléchir à la manière de les consulter (préparez vos questions, soyez précis dans vos demandes, etc...).

Après un run des attaques interne à chaque groupe, les équipes offensives échangeront leur place pour une journée afin de tester leurs attaques  sur une autre blue team qui fera un raport sur la detection tandis que les équipes redteam feront un rapport sur le résultat des attaques.
  
## Technologie
- Votre infrastructure contiendra un serveur de logs (OpenWEC)
  (voir https://www.sstic.org/2023/presentation/openwec/) réceptacle des logs de vos serveurs windows.
  


## Livrables attendus

- Un compte rendu qui contiendra une synthèse du travail accompli. Une synthèse ce n'est pas un rapport. Elle doit être la plus efficace possible en peu de pages. Elle permettra à votre client de se faire une idée précise de votre travail et d'orienter ces choix défensifs.
 
Elle ontiendra **sous forme synthétique** :
  * Un descriptif synthétique de ce que vous avez en oeuvre. (schéma, technos...)
  * Les résultats obtenus.
  * Un bilan chiffré et graphique de votre gestion du projet par personne et par tâche.
  * Un avis éclairé sur l'efficacité de votre détection avec un comparatif d'efficacité des différentes méthodes de détection.
  * Vos acquisitions personnelles et de groupes en termes de compétence avec un retour sur vos "Win/fail" pour préparer votre portfolio.

- A la suite de ce compte rendu pour délivrerez des annexes détaillant l'installation de votre environnement.

* Dépôts Git pour la partie automatisation et déploiement des agents.
* Bilan des questions posées et réponses apportées.
* Traces des installations et des configurations réalisées. Chaque annexe précisera son auteur et la durée de réalisation.

l'ensemble des matériels devra être ré-initialisé avant la fin de la SAE. Un manquement à cette règle entraînera une pénalité sur l'appréciation de vos compétences.
