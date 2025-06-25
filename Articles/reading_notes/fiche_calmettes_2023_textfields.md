# **État de l’art – REF-004**
Calmettes Maëva, Joatton Jean-Baptiste, Maudet Nolwenn et Thollot Joelle, « Exploring the Untapped Potential of Text Fields in Creative Software », New York, NY, USA, Association for Computing Machinery, coll.« IHM ’23 », 2023.
# **Résumé**
## Problème traité
Les interactions textuelles (au travers de l’interprétation d’un texte par un logiciel, dans un langage naturel ou non) ont progressivement été dévaluées dans le champ de l’IHM avec l’avénement des interfaces de manipulation directe. En effet, il sont sujets à des erreurs de syntaxe, demande certaines connaissances et prennent plus de temps (à être tapées ou compilées). Pourtant, les interactions textuelles permettent des manipulations avancées et complexes difficiles à émuler au travers des outils de manipulation direct.
### Objectif scientifique
*→ Permettre le support, par des outils de création, de pratiques créatives grâce aux interactions textuelles au sein des, déjà très répandus et standardisés, text fields.*
### Approche
- État de l’art
- *Design space* explorant les capaciés interactives des *text fields* pour la lecture/compréhension et l’écriture → Combinasion de la manipulation direxte et textuelle
- *Développement de VectorPattern, un prototype de création de motifs à l’aide d’un text field conçu pour l’écriture d’expression mathématiques*
  1. ### Contribution
     #### *Textfield design space*
     ![](Aspose.Words.94959af6-0a1c-4538-85ca-4d2268e5833f.001.png)Textfields = Intermédiaires entre : *imperative controls*, *selection controls*, *entry controls* et *display controls* les text fields sont à la fois des élements d’interface interactifs et des espaces d’écriture.

     Les listes ci-dessous reprennent chaque caractéristiques et les définissent.
     1. ##### *Objectifs des text fields*
- Compréhension de la valeur retournée et de son effet
  - + comprendre quelle propriété ou action l’input de l’utulisateur·ce change + son unité
- Compréhension des bases du langages
  - Qu’est ce qu’un input valide pour un TF qui accpete + qu’un nombre
  - Apprentissage de la syntaxe, compréhension du vocabulaire.
- Découverte et exploration du langage	
  - Comprendre les possibilités permises par le langage permet d’augmenter la créativité de l’utilisateur·ice
  - + connaître l’étendue du lange, encourager les divergences, rendre les expressions plus complexes, éviter l’effet « white field »
- Rendre plus exploitable (usable) le processus d’écriture
  - Production d’une docoumentation située
  - Facillitation du partage et de la réutilisation du travail
- Aide à l’organisation de l’écriture (Comfort de l’utilisateur·ice)
  - Interaction plus facile/naturelle (pas forcément plus rapide)
  - Processus d’écriture plus rapide, plus simple & aide pour les fautes de frappe
##### *Caractéristiques graphiques*
- Caractérisituques visuelles
  - Graphisme se limitant au champ et à son contenu
- Layout characteristics
  - Position et taille, impactant l’interface
- Utilisation d’un élement additionnel
  - Élements d’assistances ou élements « nested »
- Fonctionnalités de manipulation et d’interpreation du texte
  - Éditent directement le texte ou utilisent une sémantique spécifique
  - Dorking, hints, désactivation...
    1. ##### *État d’interaction du text field*
       Généralement les variations graphiques sont lié à l’état du text field.

       Permettent la diversification des interactions

- Rested
  - Pas d’interaction en cours, le champ écoute les évenements et son contenu peut être édité
  - Pas nécessairement visible ou dans sa forme graphique principale
- Highlighted
  - Souvent pendant la manipulation directe (*hovered* *state*)
  - N’applique pas d’autres moyen d’interaction. Très lié à des appareils de *pintpoint*.
- Focalised
  - En mode « édition » (l’utilisateur·ice écrit)
  - Peut servir d’entre deux entre highlight et l’édition (en montrant plus d’infos)
- Edited
  - Pendant la manipulation du texte (ajout de valeurs, sélection, déplacement, copier-coller, effacer du texte...)
- Selected
  - Moins commun, souvent appelé mouse/touche expanded
  - Demande une action délibérée ou spécifique de l’utilisateur·ice qui ≠ taper du texte
  - Souvent déclanché par un drag ou click sur la bordure du field, une icône, une flèche
- Locked/Disabled
  - Vérouillage du champ
  - Peut permettre de montrer de l’information/attendre une action spécifique de l’utilsateur·ice/un travail du programme
### Résultats
#### Application du text field design space à un outil de conception de motifs
L’article décrit la façon dont les chercheur·euses ont utilisé le design space pour générer des idées de charactéristiques à partir des objectifs.

Écriture d’un scénario d’usage comparant un text field classique et les possibilités de Vector Pattern à partir des différents objectifs, charactéristiques et états.

L’article défend l’idée que les text fields, discrets et déjà bien implémenté dans les logiciels, pourraient permettre beaucoup de possibilités dans le processus créatif.  

Text fields : juste milieu entre le pouvoir de la programmation et l’accesibilité de la manipulation directe (cf. Scriptographer de Jürg Lehni ou le plug-in Illustrator permettant de manipuler des objets avec du JS, bien que nombreux de ces types de projets aient pris fin… Projet récent : Glisp de Baku Hashimoto).
#### Extension du design space pour définir 5 types d’interactions permettant de passer d’un état à l’autre du text field
- En fonction de la temporalité
  - (transitoire, durable, continu)
- En fonction de la granularité des contrôles permis
  - (pré-définis, approximatifs, précis)

→ Combiner des interactions basiques et riches permet des interactions plus complexes.

- Interactions basées sur la commande (clic, tape, raccourci, commande vocale….)
  - Permet une action prédéfinie et transitoire
- bassées sur le pointeur (pointer avec un curseur, le déplacer…)
  - Souvent pour la sélection de texte et le déplacement d’objet : interactions continues permettant un contrôle approximatif mais direct
- entrée de texte (avec un clavier, dictaphone, stylet)
  - dédié à l’entrée de texte, comme suite de l’action transitoire de taper des caractères
- interaction unidimensionnelle (2 flèches, roue de la souris..)
  - Set d’actions binaires (+/-, avant/arrière...)
- interaction multidimensionnelle (4 flèches, gyroscope…)
  - Permet d’introduire plus de paramètres

![](Aspose.Words.94959af6-0a1c-4538-85ca-4d2268e5833f.002.png)
#
# **Lecture critique**
## Points forts
#### *Vector Pattern*
Les idées d’interactions sont implémentées séparement et génèrent des possibilités ne se limitant pas aux incompatibilités d’une fonctionnalité avec une autre.

Ne limite pas les interactions textuelles à des interfaces en ligne de commande mais tente encourage plutôt à développer des interactions hybrides entre interactions textuelles et manipulation directe. Cela permet de profiter du « biais d’assimilation ».

Les text fields sont déjà bien standardisés et implémentés et peuvent être augmenté facilement sans créer de changement drastique dans les affordances logicielles. Leur simplicité les rends aussi plus accessibles que les IDE.

Par rapport aux « limites » de l’écriture sous-citées :\
→ Cette friction peut tout de même être intéresante et génére de nouvelles formes.

→ Encourage l’utilisateur·ice à une maîtrise plsu experte de l’outil.
#### *Design Space*
- Ouvre à des possibles en matière d’UI
- Permet d’analyser les text fields existant comme points de départ à la génération d’idées nouvvelles
## Limites
Il semble que le design space est utile à la production d’idées dans le cas du design graphique, mais cela n’a pas encore été testé avec des designers en IHM. L’article démontre que le design space permet d’avoir de nouvelles idées sans pour autant valider ces idées avec des utilisateur·ices.

L’écriture est plus sujette aux erreurs et la courbe d’apprentissage des utilisateur·ice et plus longue.

Pose la question des prompts et de nos interactions purement textuelles dans le cadre du *machine learning*. Comment les outils d'aide à l'écriture dans les champs de texte peuvent prendre en charge des pratiques réflexives, notamment pour des outils tels que l’apprentissage automatique basés sur ceux-ci ?
#### *Vector Pattern*
Fonctionne plus sur une logique de « trials and error » que de réalisation d’un motif pensé en amont. Plus difficile à prendre en main car moins instinctif qu’un logiciel en manipulation directe (il faut comprendre le langage pour s’en servrir).

→ Peut générer de la frustration.\
` `Design Space

- Ne contient pas toutes les charactéristiques possibles et/ou existantes.
# **Lecture approfondie**
État de l’art

- Compréhension de la valeur retournée et de son effet
  - Affichage du résultat, timeline & keyframes, ralentissement de l’exécution (déconstruction du mouvement)
  - Aide visuelle
  - Favorisation des aller-retours entre l’écriture et le résultat
  - Modes hybrides d’interaction
- Compréhension des bases du langages
  - Accès intégré à la documentation
  - Documentation liée à des termes cliquables
- Découverte et exploration du langage	
  - Encourgaement à l’exploration (step by step, commentaires…)
  - Dépasser l’appréhension de la page blanche
- Rendre plus exploitable (usable) le processus d’écriture (tendent  à garder l’utilisateur·ice dans un seul mode d’interaction, avec le clavier)
  - Interactions supportant l’écriture (Google Sheets) / help pannels
  - Correction automatique, suggestion automatique, auto-completion
  - Raccourcis claviers
- Aide à l’organisation de l’écriture
  - Note taking/productivity tools → navigation dans les documents via l’interaction textuelle
Calmettes Maëva, Joatton Jean-Baptiste, Maudet Nolwenn et Thollot Joelle, « Exploring the Untapped Potential of Text Fields in Creative Software », New York, NY, USA, Association for Computing Machinery, coll.« IHM ’23 », 2023.

<a name="pagenumwizard_footer_default page style2"></a>07 / 07
