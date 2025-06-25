*État de l’art, RÈF-001*

Jalal Ghita, Maudet Nolwenn et Mackay Wendy E., « Color Portraits: From Color Picking to Interacting with Color », New York, NY, USA, Association for Computing Machinery, coll.« CHI ’15 », 2015.
# **Résumé**
1. ## Problème traité
   Les *Color Pickers* numériques n’ont presque pas évolués depuis les années 1990. Pourtant, des études montrer que les utilisateur·ices non formées ont des difficultés à sélectionner des couleurs particulières tandis que les artistes professionnels ne souhaitent pas simplement suivre des systèmes et théories prescrites.
   1. ### Objectif scientifique
      *→ Améliorer la manipulation des couleurs par les auteur·ices de médias numériques pour atteindre l’effet désiré.*
      ### Approche
- État de l’art (perception de la couleur, technique de visualisation des espaces colorimétriques, design d’outils spécialisés de manipulation de la couleur)
- Entretiens avec artistes et designers se concentrant sur la couleur et cadrage du résultat dans un « design space » : *Color Portraits*
- Vérification du design space avec des non expert·es et par l’analyse d’outils de couleur actuels
- Présentation d’un set de nouveaux outils de manipulation de la couleur testant le pouvoir génératif du design space + présentation à des utilisateur·ices comme « sonde » pour conclure  les implications, pour le design, d’outils de manipulation de la couleur plus avancés.
  1. ### Contribution
     #### *Identification de pratiques d’expert·es et développement du Design Space « Color Portraits »*
     1. ##### *Picking and Tweaking + Palettes : Manipulation des relations entre couleurs*
        *→ Développement de Palette Explorer*

        *Création de palettes interactives dans un contexte, manipulation des couleurs en contextes (une couleur, plusieurs couleurs)*

        *Story des participant·es : utiliser pour expérimenter des palettes et des website layouts*
     1. ##### *Composites : Assemblage d’élements disparates (couleur/texture…)*
        *→ Développement de Color Compositor*

        *Permet de fondre les couleurs et textures comme unités uniques décomposables et manipulables dans l’espace, en contexte, ou palette complète.*

        *Story des participant·es : Changer le type de texture en manipulant la couleur (oranges → citrons)*
     1. ##### *History : Historique de création des couleurs, de leur source, états intérmédiaires et finalité. (Non supporté par les outils de sélection de couleur)\**
        *→ Développement de Color Partner*

        *Permet de partir de deux couleurs pour générer d’autres couleurs bases sur la distance entre les noeufs colorés et le curseur. Possibilité de sauvegarder les couleurs favorites et de les réutiliser pour générer de nouvelles couleurs.*

        *Story des participant·es : Impression de « posséder » les couleurs, bien que générées par un système. Ce sont « ses » couleurs et iel ne souhaiterai pas les partager avec quelqu’un·e d’autre.*
     1. ##### *Process : la couleur comme moyen pour une fin. Manipulation directe et indirecte.*
        *→ Développement de Color Revealer*

        *Permet de comprendre les habitudes d’écriture en utilisant les couleurs pour réveler les hésitations (opacite) à l’écriture ou pour indiquer le progrès (nuance).*

        ` `*Story des participant·es : a permis de réaliser des habitudes sur le processus d’écriture (suppression d’un mot complet plutôt que de la simple faute de frappe)*
        ### Résultats
- L’interaction des utilisateur ·ices avec la couleur est plus complexe qu’une simple sélection, contrairement aux focus des outils habituels.
- L’expérimentation des *probes* avec des utilisateur·ices non spécialistes de la couleur montre que les scientifiques et ingénieur·euses ont des besoins de manipulation de la couleur similaires aux artistes et designeur·euses, confirmant la pertinence du Design Space *Color Portraits*.
- Le développement d’outils alternatifs (comme illustré par les probes) permettrait aux utilisateur·ices d’avoir des interactions plus riches avec la couleur.
- Les besoins de « picking and tweaking » ne sont pas adressés puisque déjà bien supportés par les outils existants. Parfois ces outils fonctionnent bien (surtout pour Picking and Tweaking) d’autres fois il y a des manquements (support partiel des interactions avec les palettes) et d’autres fois une absence de réponse au besoin (Composites).
###
# **Lecture critique**
## Points forts
Évaluation du Design Space avec différentes typologies d’utilisateur·ices (designeur·euses et artistes mais aussi scientifiques et ingénieur·euses) qui ont des besoins spécifiques de manipulation de la couleur.

Comparaisons d’outils existants permet de se rendre compte des manquements de ceux-ci lorsqu’il s’agit de répondre aux 5 besoins identifiés.
## Limites
La recherche en l’état n’aborde pas la question de la recommendation de couleurs par l’outil ou la possibilité de partager les couleurs générées.

Proposition de recherches supplémentaires :

- Expérimentation
  - Permettre l’exploration des relations colorées, comparaison des alternatifs et support de contraintes définies par l’utilisateur·ice
- Ownership
  - Personnalisation des couleurs, capture des étapes provisoires de création, conservation du contexte de la création de couleurs, support de la réutilisation des chaînes de création de couleur
- Partnership User-System
  - Suggestion de sous-set de couleurs par le système et guidage du système dans de nouvelles directions par l’utilisateur·ice
- Intergation
  - Combinaison d’élements divers, manipulation des composites et décomposition de ceux-ci en composants.

# Lecture appronfondie
## *Résultats*
### État de l’art
Couleur =  domaine complexe, étudié en psychologie, computer science, mathématiques, art et design…

La perception de la couleur est complexe, c’est une interprétaton du cerveau. Les artistes et designeur·euses jouent souvent d’illusions optiques pour obtenir des effets spécifiques.

- La couleur peut être représentée et visualisée de différentes façons.Coding schemes basés sur les maths ;
  - RGB (device-dependent), HSV : emphase sur la génération de couleur plus que la perception. RGB produit beaucoup de verts mais peu de rouges.
- Ou sur la perception colorée
  - CIELUV/CIELAB : perceptually uniformcolor spaces
  - coding schemes réduisant l’effort cognitif en se limitant aux capacités du système de vision humain (computer-aided color picks for representing data)
  - Couleur varient selon le média (print/screen) : CMJN et Pantone Matching System
- Beaucoup d’outils de couleur sont basés sur des algorithmes dissimulant la complexisté de la manipulation de couleur. Sans compréhension des modèles, les utilisateur·ices peuvent avoir des difficultés pour les utiliser.
  - ACE (A Color Expert) : sélectionne automatiquement les couleurs à partird’un modèle des relations fonctionelles entre composants d’un croquis de principe
  - Wang et al. : processus de colorisation interactif qui permet aux utilisateur·ice de choisir des nuances sur une roue colorée avant que le système expert ne calcule la luminosité et saturation optimale

→ Ces outils sont intéressants pour des tâches précises mais moins utiles pour les tâches créatives au sein desquelles le sutilisateur·ices définissent leurs propres règles et contraintes.

Outils de couleur interactifs :

- Web-based
  - Adobe Kuler : combinaison de couleur autour d’un thème (triades, complémentaires, à partir d’images…)
  - Sélection d’un set de couleur pour répondre à des requirements spécifiques (palettes pour les cartes, pour des couleurs simples…)

→ Avantages de la simplicité mais portée limitée

Outils innovants :

- Histomages : édition de l’image par la manipulation d’un histogramme des pixels colorés
- Poli and Reinhard
- Meier et al : Interactive color palette tools

La couleur dans le design :

- Artistes et designeur·euses ont une compréhension nuancée de la perception colorimétrique par leur ppratique intensive et leur expérience
  1. #
     ## Interaction des artistes avec la couleur
     Pratiques surprenantes :

- Choix d’une couleur incorrecte pour signifier que la couleur finale n’a pas été choisie
- Allers-retours entre artefacts physiques et couleurs numériques
  1. ### Picking and Tweaking
- Choix d’une couleur particulière, d’une source qui peut varier (espace colorimétrique, échantillon coloré...)
  - Généralement tweaked avant d’être appliquée à l’artefact
- Choix depuis un color picker commercial (échantillons trouvés sur des sites web, des palettes, des photographies, des objets physiques comme la céramique ou le textile)
  - Parfois utilisation direct de l’échantillon colorée (par exemple pour être sûr que le résultat imprimé soit le bon) mais généralement tweaked avant d’être appliqué.

La plupart des participant·es utilisent des échantillons et trouvent le color picker utile pour la modification des couleurs.
### Palettes : manipulation des relations entre couleurs
Création d’un set de couleurs cohérentes manipulées en groupe (palettes)

Activités liées au palettes :

- Comparaison d’échantillons de différentes tailles
- Superposition ou repositionnement
- Manipulation de groupe de couleurs comme faisant un
- Interaction avec les couleurs indépendemment (avec le color picker par ex. ou dans le contexte des autres couleurs.)

![](Aspose.Words.ab1fea54-b78b-4dcd-a866-7602fd4162ab.001.png)
### Composites : assemblage d’élements dispaeates
Utilisation d’élements supplémentaires (ex. textures) pour produire la couleur. Malheuresement, les outils de culeurs sont conçus pour manipuler les propriétés de couleur et ne permettent pas la création de composites couleur/texture complexes.
### Historique : Interaction avec les actions précédentes

- Tâches similaires répetées et necessité de revoir d’ancien artefacts lors de la création de nouveaux
- Étapes intérmédiaires pour explorer des chemins altrnatifs sans avoir à recommencer le processus depuis le début.

→ Besoin de sauvegarder des étapes intermédiaires lors du processus de création d’une couleur

→ (Plus rarement) sauvegarde de la source (image) des couleurs ou la finalité (palette)

Mais les color picker ont la forme d’historique la plus simple (espaces d’enregistrement des dernières couleurs mais sans contexte/source/étapes nécessaires pour les créer).

### ` `*Processus*
Pour les objets physiques : particpant·es observent des changement de couleur témoins d’états provisoires de l’artefact (ex. couleur d’un métal chauffé)

→ La couleur comme moyen

![](Aspose.Words.ab1fea54-b78b-4dcd-a866-7602fd4162ab.002.png)Suggère une opportunité intéressante pour les outils électroniques ; le changement de couleur comme révélateur des changements sous-jacents d’une activité en ligne.
Maudet Nolwenn, Jalal Ghita, Tchernavskij Philip, Beaudouin-Lafon Michel et Mackay Wendy E., « Beyond Grids: Interactive Graphical Substrates to Structure Digital Layout », Denver Colorado USA, ACM, 2017.

<a name="pagenumwizard_footer_default page style2"></a>07 / 07
