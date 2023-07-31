## Modèles de conception
### Introduction
    Les modèles de conception sont des modèles de code qui résolvent des problèmes classiques de conception de logiciels. Il ne s'agit pas de code prêt à l'emploi, mais plutôt de modèles ou de directives que vous pouvez utiliser pour créer vos propres solutions.

## Modèle de conception de référentiel
### Explication du modèle de conception
     Le Repository Design Pattern est un moyen d'organiser la logique d'accès aux données dans une application logicielle. Il fournit une interface commune pour accéder à différents types de sources de données. Ils facilitent le test de la logique de votre application
### Avantages de l'utilisation du modèle de conception
   * ça facilite les tests.
   * ça sépare la logique de données de la logique de service.
   * ça permet un échange facile de différents magasins de données.
   * ça réduit la duplication de code.
### Inconvénients de l'utilisation du modèle de conception
   * ça ajoute une couche supplémentaire d'abstraction.
   * ça peut masquer les fonctionnalités et les capacités du magasin de données sous-jacent.
   * ça peut entraîner une duplication ou une incohérence du code

## Injection de dépendance.
### Explication de l'injection de dépendance
     L'injection de dépendances est une technique de programmation qui permet à un objet ou à une fonction de recevoir d'autres objets ou fonctions dontça dépend, au lieu de les créer lui-même. De cette façon, l'objet ou la fonction n'a pas besoin de connaître les détails de la construction ou du stockage des dépendances et peut se concentrer sur sa propre logique.

### Avantages de l'utilisation de l'injection de dépendance
   * ça facilite les tests
   * ça sépare les préoccupations de construction et d'utilisation des objets
   * ça permet un échange facile des différentes implémentations des dépendances
   * ça réduit le couplage entre les classes et leurs dépendances.

### Inconvénients de l'utilisation de l'injection de dépendance
   * ça augmente la complexité et réduit les performances de l'application
   * ça masque les fonctionnalités et les capacités du magasin de données sous-jacent
   * Problèmes de performances potentiels.

## Observateur
### Explication de l'Observateur
     L'observateur est un moyen d'organiser la communication entre les objets qui ont une relation de dépendance un-à-plusieurs. ça signifie que lorsqu'un objet (l'observable) change d'état, tous les autres objets (les observateurs) qui en dépendent sont notifiés et mis à jour automatiquement.
### Avantages d'utiliser Observer
   *ça découple l'observable des observateurs.
   *ça permet l'inscription et la désinscription dynamiques des observateurs au moment de l'exécution.
   *ça prend en charge la communication de diffusion.

### Inconvénients de l'utilisation d'Observer
   * ça peut provoquer des fuites de mémoire.
   * ça peut créer des problèmes de performances.
   * ça peut introduire de la complexité et de l'ambiguïté.

## Décorateur
### Explication de l'Observateur
Le modèle de conception de décorateur est un moyen d'ajouter de nouvelles fonctionnalités à un objet existant sans modifier sa structure ou son comportement. Ce modèle est utile pour implémenter des systèmes événementiels.
### Avantages de l'utilisation de Decorator
   * ça dissocie l'objet d'origine des objets décorateurs.
   * ça permet l'enregistrement et le désenregistrement dynamiques des objets décorateurs lors de l'exécution.
   * ça prend en charge la communication de diffusion.

### Inconvénients de l'utilisation de Decorator
   * ça peut provoquer des fuites de mémoire.
   * ça peut créer des problèmes de performances.
   * ça peut introduire de la complexité et de l'ambiguïté.

## Conclusion
     Les modèles de conception sont essentiels dans le développement backend moderne car ils fournissent une approche structurée pour résoudre les problèmes courants. L'utilisation de modèles de conception offre de nombreux avantages comme mentionné ci-dessus.