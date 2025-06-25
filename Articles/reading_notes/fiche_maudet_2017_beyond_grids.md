*État de l’art, RÈF-003*
# **Résumé**
1. ## Problème traité
   Les outils de mise en page traditionnels s’appuient sur la grille et sous entendent que la production est statique. \
   L’augmentation des appareils interactifs coincide avec un besoin de maquettes gérant des formats variables. Il y a aussi de nouveaux médias (blogs, magazines en ligne).

   *→ Les flux d’information continus et la diversité des médias créent de nouvelles contraintes et opportunités pour la structuration de contenu visuel, non compatibles avec la simple notion de grille.*
   1. ### Objectif scientifique
      *→ Concevoir un outil qui supporte les contraintes et possibilités du design graphique contemporain, en particulier les maquettes pour des médias numériques.*
      ### Approche
      #### *Exploration*
- Comprendre comment les designeur·euses réagissent au changement de paradigme médias statiques vs multimédia (État de l’art + entretiens et analyse des résultats)
  - How do they create structures and processes that solve the problems of the contemporary design landscape ? Do they go beyond the grid ?
#### *Characterization*
- Proposer un cadre descriptif (*graphical substrates*) pour définir les structures allant au-délà de la grille
- Développement de deux *probes* (sondes) et analyse de leur appropriation par des designeur·euses
- Développement de *StyleBlocks*
  1. ### Contribution
     Jusque ici, études se concentrant sur les DG montrent les aspects sociaux et matériels du design. Ici, auteur·ices plus intéressées par les *pratiques entourant la première phase de mise en page du contenu.* Études pré-existantes se concentrant sur les premières phases : *Démontrent le rôle critique de la structuration dans les premières phases du design mais offrent peu d’exemples sur comment les designeur·euses accomplissent cela.*

     L’article propose de premières pistes de réification des substrats graphique par le code.
     ### Résultats
     La réification des substrats graphiques par le code ouvre un nouveau champ des possibles aux designeur·euses graphiques qui font de la mise en page.

     Le développement de *probes* a permis d’ouvrir des conversations sur ces sujets et de faire naître de nouvelles idées qui pourraient permettre d’étendre la réification des substrats graphiques et leur part d’interactivité.

     Enfin, le développement du prototype *StyleBlocks* a permis de combiner et d’augmenter les *probes* en repensant les feuilles de styles CSS comme substrats graphiques interactifs. Le prototype illustre au travers du scenario d’usage le pouvoir génératif d’une réification complète des substrats dans les outils de DG.

     Le papier propose aussi des pistes de recherche pour la suite : la diversification des représentations graphiques des substrats plus expressives (ex. les ratios sous forme de rectangles) et l’exploration d’autres substrats graphiques (définir un vocabulaire plus large que ceux déjà explorés).
     # **Lecture critique**
     ## Points forts
     Méthodologie au plus près des besoins des expert·es : entretien, analyse puis proposition de *probes* pour ouvrir à de nouvelles conversations/idées pour le développement d’outils de création graphique. Cette méthodologie ouverte a permis de proposer un protoype au plus proches des usages réels, lesquels dépassent les fonctionnalités des logiciels traditionnels, et ce malgré que celui-ci ne réponde pas encore à la totalité des besoins.

     1. #### *Styleblock*
        Le prototype illustre au travers du scenario d’usage le pouvoir génératif d’une réification complète des substrats dans les outils de DG.

- Extension du vocabulaire d’*inputs* et *outputs*
- Plus de flexibilités dans la réification
- Allers-retours entre mise en page et substrats graphiques
## Limites
Le papier explore différents substrats graphiques qui sont facilement réifiables par le code au travers de relations de réseau et de tuyaux. Ils permettent un équilibre entre pouvoir et simplicité des substrats. Il serait cependant pertinent de travailler sur un plus large éventail de substrats.
1. #### *Styleblock*
   Limité aux propriétés spécifiées dans le prototype sauf si on lui permet d’accepter les *external inputs.*

   Conditions plus complexes restent un challenge : difficile de tweak ET conserver une relation.

   Permet l’édition de contenu dans des blocs existants mais n’applique pas automatiquement les blocs au nouveau contenu. Le support des classes CSS permettrai de régler le problème.

   # Lecture appronfondie
   ## *Résultats*
   ### État de l’art
- Soutien de la création de maquette par les novices
- Amélioration des pratiques de designeur·euses
- Compréhension des pratiques de designeur·euses (limité aux aspects sociaux/matériels)
- Définition des façons de structurer la mise en page par l’étude des pratiques de 12 designeur·euses
  - Entretiens & analyse des données avec *StoryPortraits* + vérification des détails avec les participant·es. *Grounded theory approach* pour catégoriser les mots-clés de ces *stories* pour les organiser dans un cadre descriptif.
  - *Substrats graphiques* = structures sous-jacentes pour la construction de la mise en page. Le changement du substrat fait évoluer la mise en page.	
    1. ### Substrats graphiques
       Les substrats se basent sur des concepts, contenus ou contextes (*inputs*) qui deviennent ensuite des propriétés spatiales ou temporelles(*outputs*). Il y a aussi d’autres *outputs* remarqués comme la typographie ou la couleur ?

       ![](Aspose.Words.73ee70cf-f36f-4cde-a542-7f4404598387.001.png)

- Compréhension des substrats graphiques mis en place par les participant·es et la façon dont i·els intéragissent avec ceux-ci (Réutilisation, Adaptation)
### Réification des substrats graphiques
- Substrats restent des idées/concepts
  - Objectif de la réification : aider les designeur·euses à transformer leurs substrats conceputels en outils logiciels manipulables. (= réifier les règles des substrats pour qu’elles puissent être executées par un programme ou un·e autre DG)
  - Tous les substrats ne sont pas toujours réifiables, où difficiliement (substrats basés sur une ambiance, un style)
  - Les outils actuels offrent un support limité des substrats graphiques
  - Nécessité de gérer les substrats manuellement plutôt que de les exprimer dans l’outil directement
  - Difficultés pour le partage des substrats entre designeur·euses
- Utilisation du code pour réigier les substrats graphiques
  - 1/2 participant·es ont entièrement ou partiellement implementé du code dans leurs projets (17 en tout dont 6 pour des artefacts imprimés). Trois approches ont été remarquées.
    - Génération d’*inputs* plus divers (règles codées puis appliquées par le système en fonction de différents paramètres)
    - Application automatique de substrats graphiques(partenariat entre DG et programme qui permet aux DG de passer plus du temps sur l’exploration et la création de substrats plutôt que les tâches chronophages d’applications de substrats sur chaque élements + ppermet de générer une infinité de mises en pages unique en fonction des règles pré-établies)
    - Implication des lecteur·ices ou d’autres designeur·euses dans la création de mise en page (choix du format print par les lecteur·ices, mises en pages interactives qui réagissent aux actions des lecteur·ices…)
#### L’ajout du code offre des possibilités de réification des substrats graphiques (mise en page print traditionelle + contenu interactif) MAIS tous lles designeur·euses ne veulent/peuvent pas programmer et les outils actuels permettent seulement seulement de réifier des substrats simples. *L’article défend l’idée que nous avons besoin d’outils de plus haut niveaux qui supportent la réification des substrats graphiques.*
### Probes (sondes) de réification des substrats graphiques + expérimentation des probes
→ Création de deux sondes logicielles inspirées par les résultats de l’étude, en particulier les raisons d’utilisation du code pour la réification des substrats graphiques.

Objectif ≠ gérer tous les substrats\
Objectif = inspirer de nouvelles possibilités pour la conception d’outils gérenant des mises en pages innovantes
#### *Contextify*
Modification des mises en page en fonction des préférences des lecteur·ices et des environnements de lecture (Nuit/Jour et Preview/Vue complète)
1. ##### *Résultats des expérimentations :*
- « Nouvelle forme de pouvoir édioriale » pour le·a DG : permettre d’adapter la mise en page à différents besoins (différentes façons d’apprendre, différents métiers consultant un document…)
- Simplification des vues multiples en interagissant avec l’outil plutôt qu’en codant
#### *Linkify*
Réification des relations spatiales des élements en fonction de propriétés dynamiques du contenu (Création de relation entre deux élements et leurs propriétés : largeur, position, taille de la fonte ou nombre de caractères. Les propriétés évoluent selon des paramètres réifiés.)
##### *Résultats des expérimentations :*
- « Interface entre designeur·euses et développeur·euses » en testant la mise en page sur plusieurs types de pages plutôt que d’attendre que son·sa collègue développeur·euse implémente les nouvelles décisions
- Permettre de nouvelles façons plus organiques, moins linéaires, d’organiser le contenu
- Permettre de créer de nouvelles mise en page sans avoir à tout redesigner systèmatiquement (car la mise en page dépend des relations entre élements)
### Extension des substrats graphiques à partir des retours des participant·es
#### *Généralisation – Étendre les inputs*
Possibilité de multiplier les contextes différents (car limités à quatres scénarios sur le probe)

- En fonction du contexte (localisation, météo, son ambiant, temporalité…)
- En fonction des besoins des lecteur·ices (âge, handicaps, types de mémoires, urgence de lecture)
- En fonction des types de lecteur·ices ou de métiers

Possibilité de multiplier les propriétés (limitées à 5 sur le probe Linkify)

- Ajout de propriétés (espace blanc, opacité…)
- Accès à des propriétés ≠ du contenu (ex. du viewport)
#### *Réification  – substrats graphiques et objets interactifs*
Envie des participant·es d’avoir plus de façon d’intéragir avec les substrats

- Possibilité de les réutiliser entre plusieurs projets
- Avoir plus de contrôle sur les liens entre objets : ratios absolus/relatifs, définition des limites…
## Styleblocks : combination et extension des probes en repensant les stylesheets CSS en tant que substrats graphiques interactifs.
CSS supporte beaucoup de propriétés mais reste très statique, d’où l’intérêt du Javascript pour les projets. Langage SASS : supporte des constructions de hauts-niveau (variables, expressions…) mais génère tojours des feuilles de style statiques.

Le prototype illustre au travers du scenario d’usage le pouvoir génératif d’une réification complète des substrats dans les outils de DG.

- Extension du vocabulaire d’*inputs* et *outputs*
  - Plus de propriétés accessibles mais limité aux propriétés accessibles en SS puisqu’on se sert de ce langage
  - Limité aux propriétés spécifiées dans le prototype sauf si on lui permet d’accepter les *external inputs.*
- Plus de flexibilités dans la réification
  - Permet lestweaks en utilisant les rations et limites.
  - Substrats indépendants du contenu, réutilisables et combinables
  - Conditions plus complexes restent un challenge : difficile de tweak ET conserver une relation
- Allers-retours entre mise en page et substrats graphiques
  - Manipulation du substrats et de la mise en page finale dans le même *workflow*
  - Possibilité de faire des mise en page exemple, des réifications, de façon interchangeable (l’une après les autres)
  - Fabrication et itération rapide d’un substrat de façon automatique
  - Point à améliorer : permet l’édition de contenu dans des blocs existants mais n’applique pas automatiquement les blocs au nouveau contenu. Le support des classes CSS permettrai de régler le problème.
Maudet Nolwenn, Jalal Ghita, Tchernavskij Philip, Beaudouin-Lafon Michel et Mackay Wendy E., « Beyond Grids: Interactive Graphical Substrates to Structure Digital Layout », Denver Colorado USA, ACM, 2017.

<a name="pagenumwizard_footer_default page style2"></a>07 / 07
