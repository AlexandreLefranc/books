# Chapitre 1 - Professionnalisme

- Etre responsable de son travail
- Assumer ses erreurs et vouloir les réparer
- Ne pas livrer dans la précipitation en sautant des étapes (les tests par exemple)
- Ne faut pas nuire au fonctionnement du programme
- Etre confiant sur le bon fonctionnement du logiciel => tester
- Ne pas livrer (ou envoyer au service QA) un logiciel dont on sait qu'il a des bugs
- Ne pas nuire à la structure du code source
- Etre responsable de sa carrière et de son évolution. Ne rien attendre de la part de l'employeur.
- Consacrer du temps personnel pour travailler ses compétences de programmation
- Apprendre continuellement
- Pratiquer des katas
- Travailler avec d'autres personnes et coder en groupe
- Transmettre aux autres
- Connaitre le domaine d'application de son logiciel et comprendre les demandes clients
- Etre humble

# Chapitre 2 - Savoir dire NON
# Chapitre 3 - Savoir dire OUI
# Chapitre 4 - Coder

- Ne pas coder la nuit => Il faut garder de la discipline sur le sommeil
- Eviter la zone de flow => Manque de recul sur le code
- Eviter de coder en musique => Distraction
- Accepter d'être intérrompu
- Coder en binôme a de nombreux bénéfices
- Faire des activités créatives: Lire des livres, etc
- Produire beaucoup de bugs est non professionel => Adopter une méthodologie pour réduire ça (TDD)
- Bloqué ? Fatigué ? Il ne faut pas s'acharner. Plutôt faire une pause, une douche, etc...
- Essayer d'estimer honnetement
  - Le meilleur cas
  - Le cas normal
  - Le pire cas
- En cas de retard, communiquer le plus tôt possible
- Résister à la pression des supérieurs et se tenir aux estimations
- Ne pas accepter de faire des heures supplémentaires sauf si
  - c'est personnellement acceptable ET
  - c'est limité dans le temps ET
  - le chef a un plan de secours si l'effort supplémentaire ne suffit pas
- Ne jamais dire qu'on a finis si c'est n'est pas le cas => Avoir une définition indépendant de l'état d'achèvement: Des tests d'acceptations
- Aider les autres avec bonne volonté. Proposer son aide
- Accepter l'aide des autres. Savoir demander de l'aide
- Si on est sénior, partager avec les juniors. Si on est junior, chercher le partage de séniors

# Chapitre 5 - TDD

- Les 3 lois du TDD
  - Ecrire du code de tests en premier
  - Arrêter d'écrire du code de test lorsque le test échoue
  - Ecrire du code de production uniquement pour faire réussir le test
- Avantages
  - Certitude de ne pas avoir généré de régression
  - Faible taux d'injection de défauts
  - Courage et confiance pour refacto le code
  - Documentation par l'exemple
  - Privilégie une bonne approche de conception
 
# Chapitre 6 - Entrainement

- Un développeur doit s'entrainer pour rester performant.
- Katas : un problème dont on connait la solution visant à rendre naturel et fluide sa résolution.
- Wazas : un kata fait à 2. Une personne écrit les tests. L'autre écrit le code.
- Randori : Un problème à plusieurs personnes. Chacun écrit le code pour passer le test et écrit un test. La personne suivante fait passer le test et écrit un nouveau test... etc
- Participer à des projets open-source dans un language différent que celui pour lequel on est payé.
- L'entrainement se fait sur le temps personnel. Par le temps professionnel.

# Chapitre 7 - Tests d'acceptation et recette

- La communication entre développeur et client est souvent problématique. Surtout vis-à-vis des exigences, du cahier des charges.
- Inutile de définir des exigences trop précises trop tôt. Elles changeront. Il faut estimer avec des plages d'incertitudes.
- Lorsqu'on définit des exigences, il peut y avoir des ambiguïtés. Pour lever ces ambiguïtés, il faut réaliser des tests d'acceptations.
- Les tests d'acceptations sont les tests réalisé entre le développeur et les parties prenantes. Lorsque les tests d'acceptations passent, le travail est fini.
- Le travail est fini lorsque le code est écrit, tous les tests passent, le QA a accepté le produit, les parties prenants ont acceptées le produit.
- Les tests d'acceptations doivent être automatisés.
- Le développeur ne commence à implémenter une fonctionnalité que lorsque les tests d'acceptations sont prêts.
- Lorsque des tests d'acceptations semblent absurdes ou trop complexes, il faut communiquer avec l'auteur des tests pour trouver une solution.

# Chapitre 8 - Stratégies de test

- Il faut rédiger des tests. Mais avant il faut mettre en place une stratégie de tests.
- L'objectif est que les QAs soientt bredouille.
- Les QAs doivent spécifier et tester les happy et unhappy paths.
- Les QAs doivent faire des tests manuels d'exploration pour vérifier le comportement effective du système.
- Tests unitaires
  - Idéalement écrit avec la méthode TDD.
  - Révèle les intentions du programmeur.
  - Couverture de code proche de 100%
- Test des composants
  - Correspond aux tests d'acceptations
  - Test des règles métier
  - Rédigé par les QAs en collab avec le métier
- Tests d'intégration
  - Lorsqu'il y a plusieurs composants
  - Test l'intégration des différents composants entre eux
  - Rédigé par les architectes système et exécuté périodiquement
- Tests système
  - Identique aux tests d'intégration mais en prenant en compte tous les composants = le système
  - Confié aux architectes ou responsables techniques
- Tests manuels d'exploration
  - Pas automatisé et pas scripté
  - Explorer le système pour trouver des bizarreries
  - Tente de reproduire le comportement d'un utilisateur 

# Chapitre 9 - Gestion du temps

## Réunions

- Assister seulement aux réunions qui ont un intéret immédiat
- Aller uniquement au réunions avec un ordre du jour et objectif
- Partir poliment si la réunion n'a plus d'intérêt

## Concentration

- Bien dormir
- Faire des exercices physiques
- Faire des pauses

## Blocs de temps

- Travailler sans discraction pendant 25 mins puis faire une pause de 5 mins
- Tous les 4 cycles, faire une pause de ~30 mins

## Autres points

- Ne pas se trouver des excuses pour ne pas faire une tâche désagréable
- Lorsqu'on voit qu'on se dirige vers une impasse ou un bourbier, il faut savoir faire marche arrière le plus tôt possible.

# Chapitre 10 - Estimations

- Un engagement doit être tenu
- Une hypothèse est représenté par une loi de probabilité
- Une estimation doit être une hypothèse, pas un engagement

## Technique PERT (Program Evaluation and Review Technique)

- Il s'agit une méthode d'estimation des delais

O = Estimation très optimiste;
N = Estimation nominale;
P = Estimation très pessimiste

$$ \mu = \frac{O + 4N + P}{6} $$

$\mu$ est la durée de la tâche attendue

## Technique d'estimation des tâches

Demander plusieurs avis sur une estimation est toujours mieux

- [Estimation de Delphes à large bande](https://fr.wikipedia.org/wiki/M%C3%A9thode_de_Delphes)
- Les doigts de vote : estime avec les doigts (0 à 5) et on discute en cas de désaccord
- Planning Poker : Variante populaire des doigts de vote avec des valeurs prédéfinie
- Estimation d'affinités

## Loi des grands nombres

- On obtient de meilleurs estimations si on divise une grande tâche en plusieurs petites tâches

# Chapitre 11 - Pression

## Eviter la pression

- Eviter de s'engager si on est pas sûr
- Garder une discipline de code, même au cours d'une crise

## Gérer la pression

- Inutile d'augmenter démesurément le volume horaire
- Communiquer avec les collègues et supérieurs
- Garder une discipline de code
- Demander de l'aide et coder en binôme

# Chapitre 12 - Collaboration et coopération

- Ne pas oublier l'objectif de l'entreprise
- Il est important de travailler avec les autres programmeurs
  - Considérer le code comme une propriété collective. Il n'appartient pas à celui qui l'a écrit.
  - Travailler en binome pour être plus efficace, et partager les connaissances
