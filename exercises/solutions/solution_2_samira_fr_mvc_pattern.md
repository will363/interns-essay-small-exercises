# Introduction et définition des patrons MVC
  Les modèles de conception MVC sont également connus sous le nom de Model-View-Controller. Il s'agit d'un modèle architectural courant utilisé pour concevoir et créer les interfaces et la structure d'une application. Il s'agit également d'un modèle d'architecture logicielle pour la mise en œuvre d'interfaces utilisateur. Le MVC est un modèle architectural qui sépare une application en 3 composants logiques principaux : le modèle, la vue et le contrôleur. Chacun de ces composants est conçu pour gérer des aspects de développement spécifiques d'une application. MVC est l'un des frameworks de développement Web standard les plus fréquemment utilisés pour créer des projets évolutifs et extensibles.

  # Composant MVC
  Il existe trois composants MVC qui sont,
  -Modèle : les classes de modèle sont utilisées pour implémenter la logique des domaines de données. Ces classes permettent de récupérer, d'insérer ou de mettre à jour les données dans la base de données qui lui est associée. Le composant de modèle peut soit représenter les données transférées entre les composants de vue et de contrôleur, soit toute autre donnée liée à la logique métier. exemple; un objet client récupérera les informations client de la base de données, les manipulera et les mettra à jour dans la base de données ou les utilisera pour afficher des données

  -View : le composant de vue est utilisé pour toutes les applications logiques de l'interface utilisateur. De plus, les vues sont utilisées pour préparer l'interface d'une application. En utilisant l'interface, les utilisateurs interagissent avec l'application. Par exemple, la vue client inclura tous les composants de l'interface utilisateur tels que les zones de texte, les listes déroulantes, etc. avec lesquels l'utilisateur final interagit.

  -Controller : les classes de contrôleur sont utilisées pour répondre aux demandes de l'utilisateur. Les contrôleurs agissent comme une interface entre les composants de modèle et de vue pour traiter toute la logique métier et les demandes entrantes, manipuler les données à l'aide du composant de modèle et interagir avec les vues pour rendre la sortie finale. Les classes de contrôleur exécutent l'action des demandes de l'utilisateur. Ces classes fonctionnent avec des classes de modèle et sélectionnent la vue appropriée qui doit être affichée à l'utilisateur en fonction des demandes de l'utilisateur. Exemple, le contrôleur client gérera toutes les interactions et entrées de la vue client et mettra à jour la base de données à l'aide du modèle client

  # Caractéristiques d'un modèle MVC
    L'architecture de modèle MVC est essentiellement une architecture à 3 couches. Il sépare les caractéristiques d'application. Sa première couche est liée à la logique d'entrée de l'utilisateur, la deuxième couche est liée à la logique métier et la troisième couche est utilisée pour implémenter l'interface utilisateur. Le modèle MVC fournit la possibilité de développement parallèle. Cela signifie que chaque couche de l'application est indépendante l'une de l'autre, c'est-à-dire que 3 développeurs ou plus peuvent travailler simultanément sur une seule application.

    # Avantages des modèles MVC
- Organise une application Web de grande taille
    Comme il y a ségrégation du code entre les trois niveaux, il devient extrêmement simple de diviser et d'organiser les applications Web (qui doivent être gérées par de grandes équipes de développeurs). Le principal avantage de l'utilisation de ces pratiques de code est qu'elles aident à trouver rapidement des portions de code spécifiques et permettent d'ajouter facilement de nouvelles fonctionnalités.

- Prend en charge l'invocation de méthode asynchrone (AMI)
   Étant donné que l'architecture MVC fonctionne bien avec Javascript et ses frameworks, il n'est pas surprenant qu'elle prenne également en charge l'utilisation d'AMI, permettant aux développeurs de créer des applications Web à chargement plus rapide.

- L'architecture MVC nous aide à maîtriser la complexité des applications en la plongeant dans ses 3 composants

- MVC utilise le modèle de contrôleur frontal. Le modèle de contrôleur frontal gère les multiples demandes entrantes à l'aide d'une seule interface (contrôleur). Le contrôleur frontal fournit un contrôle centralisé. Nous devons configurer un seul contrôleur dans le serveur Web au lieu de plusieurs.

# Outils et architecture utilisés dans MVC
 Il existe de nombreux outils et technologies utilisés dans MVC qui peuvent être utilisés pour développer des applications Web à l'aide de l'architecture MVC

 # Outils
 Visual studio, serveur MySQL, My SQL workbench, net beans, serveur Glassfish

 # Les technologies
 HTML, CSS, JQUERY, AJAX pour la conception
Pages servlet et Javaserver utilisées avec les net beans
Technologies de beans Java d'entreprise

# Conclusion
L'architecture de modèle MVC et les technologies intégrées telles que JSP, Servlet et EJB sur la plate-forme J2EE ont simplifié le processus de développement d'applications Web. Nous pouvons créer une application Web évolutive, transparente et portable à l'aide de l'architecture MVC. L'architecture MVC fournit le concept de développement parallèle car elle divise la logique d'application en trois couches, de sorte que chaque développeur différent peut travailler simultanément sur ces trois
couches d'une même application Web.

La première couche de l'architecture MVC est le modèle utilisé pour interagir avec la base de données. C'est essentiellement la couche logique de notre application qui est utilisée pour insérer, récupérer et mettre à jour les données dans la base de données. La deuxième couche est la vue qui est liée à l'interface utilisateur, à travers laquelle les utilisateurs interagissent avec notre application, comment notre application sera présentée au utilisateurs, il est essentiellement utilisé pour le développement frontal. Le troisième plus tard de l'architecture MVC est le contrôleur qui est utilisé pour obtenir les entrées des utilisateurs. Il contrôle les mises à jour de l'état de l'objet modèle et l'affichage des données aux utilisateurs en fonction des entrées de l'utilisateur. L'utilisateur peut demander à notre application et obtenir une réponse via la couche contrôleur.