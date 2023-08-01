# **Patron de conception (Dépot, injection de dependence, Decorateur and Observateur)**

Les design patterns sont des patron ou modele de conceptions qui rendent simple le processus de codage, ameliore la maintenabilter et promouvoir la reutiisation du code.
Il aide les developeurs a ecrire les code plus efficassement, evolutif et adaptable sans oublier qu'il est tres benefique lorsqu'uon l'utilise dans un project en groupe.

Il existe plusieurs type de design pattern:

## Le modèle repositoir

le repositoir est un modèl de conception qui fournit une couche d'abstraction entre l'accès aux données et le reste de l'application. Il sépare la logique qui récupère les données du stockage des données, offrant une approche plus modulaire du développement logiciel. 
Dans le modèle depot, un repos agit comme un médiateur entre le stockage de données et la logique d'application. Il fournit un point d'entrée unique pour récupérer et manipuler les données, permettant au reste de l'application d'être découplé des spécificités du stockage des données. Cela facilite le changement du stockage des données sans affecter le reste de l'application.

### Avantages 

 La partie logique de l'application est séparée du stockage des données, ce qui facilite le test et la maintenance de chaque composant séparément. Cela permet également de réutiliser la logique applicative avec différentes couches de stockage de données.

Il peut améliorer les performances en réduisant le nombre d'appels à la couche de stockage de données. La logique d'accès aux données étant encapsulée dans le référentiel, il est possible d'optimiser les requêtes et de réduire le nombre d'appels à la base de données.

Il peut améliore les performances en réduisant le nombre d'appels à la couche de stockage de données.

Dans l'ensemble, le Repository Pattern est un outil utile pour créer des systèmes backend évolutifs, maintenables et efficaces. Il sépare les préoccupations et permet une approche plus modulaire du développement logiciel, ce qui facilite le test, la maintenance et la modification de la base de code. 

## L'injection de dependence

Le modèle d'injection de dépendance (DI) est un modèle de conception qui permet la création de composants logiciels faiblement couplés. Il est utilisé pour réduire le couplage entre les composants et améliorer la flexibilité, la testabilité et la maintenabilité du code.

Dans le modèle d'injection de dépendances, les dépendances sont injectées dans un composant plutôt que d'être crées dans le composant. Cela permet de créer des composants indépendamment de leurs dépendances, ce qui facilite le remplacement ou la modification des dépendances sans affecter le composant lui-même.

Il existe trois principaux types d'injection de dépendance : l'injection de constructeur, l'injection de propriété et l'injection de méthode. 

L'injection de constructeur consiste à transmettre des dépendances à un composant via son constructeur.

L'injection de propriété implique la définition de dépendances via les propriétés publiques du composant.

L'injection de méthode consiste à transmettre des dépendances aux méthodes du composant.

### Avantages

Il améliore la testabilité du code. 

Il rend le code plus flexible et maintenable. En réduisant le couplage entre les composants, il est plus facile de modifier ou de remplacer des composants sans affecter le reste de l'application.

Le modèle d'injection de dépendance est un outil utile pour créer des systèmes principaux évolutifs, maintenables et efficaces. Il réduit le couplage entre les composants et améliore la flexibilité, la testabilité et la maintenabilité du code.

## Modèle obervateur

Pattern observateur est un modèle de conception qui permet à un objet (le sujet) d'avertir d'autres objets (les observateurs) lorsque son état change. Il permet aux objets de communiquer entre eux sans avoir une connaissance directe de l'existence de l'autre.

Dans le modèle d'observateur, le sujet maintient une liste d'observateurs et les avertit lorsque son état change. Les observateurs peuvent alors agir en fonction du changement d'état du sujet. Cela permet une relation faiblement couplée entre le sujet et les observateurs, ce qui facilite la modification ou l'extension du système.

### Avantages

Il améliore la modularité et la flexibilité du code. En séparant le sujet et les observateurs, il est possible d'ajouter ou de supprimer des observateurs sans affecter le sujet, ou d'ajouter de nouveaux sujets sans affecter les observateurs existants.

Il peut améliorer les performances du système. 

Dans l'ensemble, l'Observateur permet une relation faiblement couplée entre les objets, améliorant la modularité et la flexibilité du code. Il peut également améliorer les performances du système en réduisant le nombre de notifications.

## Patron Decorateur

Le motif décorateur est un motif de conception qui permet d'ajouter un comportement à un objet individuel, de manière statique ou dynamique, sans affecter le comportement des autres objets de la même classe. Il est utilisé pour ajouter des fonctionnalités aux objets au moment de l'exécution, plutôt qu'au moment de la compilation.

Dans le patron decorateur, une classe de décorateur est utilisée pour envelopper l'objet d'origine. La classe décorateur a la même interface que l'objet d'origine, ce qui lui permet d'être utilisé de la même manière. La classe de décorateur ajoute ensuite un comportement à l'objet d'origine en déléguant une partie de son travail à l'objet enveloppé et en ajoutant son propre comportement.

### Avantages  

Il permet l'ajout dynamique de fonctionnalités aux objets. Cela peut être utile dans les situations où le comportement d'un objet doit être modifié au moment de l'exécution, ou lorsque le comportement d'un objet doit être étendu sans modifier son interface.

Il peut améliorer la maintenabilité du code.

Dans l'ensemble, le Decorateur est un outil qui permet l'ajout dynamique de fonctionnalités aux objets, améliorant la flexibilité et la maintenabilité du code.

## Conclusion
Les modèles de conception sont essentiels dans le développement backend moderne car ils fournissent une approche structurée pour résoudre les problèmes courants. L'utilisation de modèles de conception offre de nombreux avantages, notamment la réutilisation du code, l'évolutivité, la maintenabilité, la réduction des erreurs et l'amélioration des performances.