---
author: Emmanuel Château-Dutier
since: 2016-01-02
---



# Nous avons besoin d’un nouveau éditeur XML libre et open source

Fin 2015, j’avais rejoint avec enthousiasme le travail de mon collègue Marcello Vitali-Rosati qui voulait produire un éditeur XML car je pense depuis plusieurs années que nous avons réellement besoin de proposer une interface graphique facile d’utilisation pour faciliter l’édition de document XML[1]. La production d’un tel éditeur anime depuis longtemps la communauté XML. Il y a quelques années déjà, Daniel Fekete avait annoncé qu’il était en train de développer un logiciel de ce type destiné à remplacer [Millefeuilles](http://millefeuille.gforge.inria.fr) sur le modèle d’un [EtherPad](http://etherpad.org), mais sans suite. La réalisation d’un tel éditeur avait un moment fait partie des tâches que se proposait de réaliser le projet [Biblissima](http://www.biblissima-condorcet.fr/en/news/survey-xml-editors-teiead), mais ils y ont renoncé pour l’utilisation d’une solution commerciale déjà existante ([XMLmind XML Editor](http://www.xmlmind.com/xmleditor/)). Entre temps, d’autres éditeurs commerciaux ont largement fait évoluer leurs logiciels pour proposer des modes auteurs de type wysiwig dont la simplicité d’utilisation n’a rien à envier aux logiciels de traitement de textes en ligne comme [Google docs](https://docs.google.com) ou [Microsoft Office Online](https://products.office.com/fr-ca/office-online/documents-spreadsheets-presentations-office-online). D’ailleurs leur interface est en grande partie conçue d’après leur modèle. Pour ne citer que quelques uns d’entre eux, mentionnons par exemple la très belle interface de [Xeditor](http://www.xeditor.com/portal), de [FontoXML](https://fontoxml.com), de [SDL Xopus](http://www.sdl.com/solution/knowledge-delivery/xml-publishing-xopus/) ou celle proposée par [oXygen](https://www.oxygenxml.com/xml_web_author.html). En tous les cas, ces applications démontre aujourd’hui (s’il le fallait encore) qu’il est possible de concevoir des interfaces graphiques faciles d’utilisation sans renoncer en rien à la richesse sémantique et contextuelle offerte par les technologies XML.

On peut depuis se féliciter que le travail ait bien avancé sur ce projet d’éditeur dénommé Stylo. Pour autant, je ne suis pas vraiment satisfait par les orientations prises par ce projet. Même si celles-ci sont tout à fait justifiées et pragmatiques. Comme il s’agissait notamment de permettre principalement la production d’articles pour des publications académiques, notamment au [format Érudit](http://www.erudit.org/xsd/article/3.0.0/doc/), le projet a rejoint une initiative qui avait émergée autour de la librairie JavaScript [Substance](http://substance.io). Celle-ci avait principalement le mérite de bénéficier du support financier et institutionnel de plusieurs acteurs de poids dans le domaine de l’édition scientifique comme [PKP](https://pkp.sfu.ca) ou le [Collaborative Knowledge Foundation (CoKo)](http://coko.foundation/). Au printemps, elle a aussi été rejoint par Érudit dans un consortium spécial dans le cadre de la refonte de leur chaîne éditoriale.

Pourquoi je pense cependant que nous avons toujours besoin d’un éditeur XML de ce genre ? Dire qu’il n’existe pas actuellement de solution de ce type libre et open source pourrait en soi suffire, mais ce n’est pas seulement cela. En effet, même les solutions actuellement proposées ne sont pas encore tout à fait satisfaisantes. Parfois du fait même que n’étant pas libre, cela empêche leur personnalisation pour répondre aux besoins que nous identifions ici. Mais aussi parcequ’elles copient encore trop, de notre point de vue, le modèle d’interface qui s’est imposé avec des logiciels de traitement de textes comme Microsoft Word.

Du côté des éditeurs XML libres on est bien à la peine. Mis à part [Emacs](https://www.emacswiki.org/emacs/RELAX_NG) qui dispose d’un package compatible avec les dernières technologies de [schema XML](https://www.w3.org/XML/Schema) (notamment [RelaxNG](http://relaxng.org)), sur [Vim](http://www.vim.org/scripts/script.php?script_id=1397) on ne dispose d’aucun outil correct pour éditer des fichiers XML d’après un schema, et ne parlons même pas de ce qui est pour le moment disponible sur [Atom](https://atom.io/search?utf8=✓&q=xml) qui est pour le moins rudimentaire. Le seul projet entièrement libre et open source qui offre actuellement une comptabilité avec les technologies de schema est [XML copy-editor](http://xml-copy-editor.sourceforge.net) mais qui n’est plus un projet très actif. Il y a quelques années, une tentatives avait été conduite par Mith avec [Angles](http://mith.us/angles/) mais il ne semble pas que celle-ci ait vraiment prospéré.

Est-ce à dire qu’il n’y a pas d’utilisateurs ? De toute évidence, le cas d’usage actuel de XML est particulier, il s’agit essentiellement de l’édition de texte structuré. Dans ce domaine, aucune autre technologie que XML ne répond de manière réellement adéquate aux besoins de structuration et de balisage du texte. Pour ce cas d’usage, le modèle de données de XML propose un contenu mixte qu’aucun autre format informatique ne propose actuellement. Par ailleurs, les technologies XML offrent des fonctionnalités avancées pour le contrôle de conformité des documents et permettent de construire un outillage avancé et efficace pour accompagner la productions des documents avec les technologies de schémas. Si l’édition classique peut se contenter pour le moment de HTML, c’est très loin d’être le cas dans le domaine de l’édition savante ou de la documentation technique où la [Text Encoding Initiative](http://www.tei-c.org/index.xml) ou [DocBook](http://docbook.org) sont encore très largement utilisés par exemple. Mais surtout, l’apparente complexité associée à la saisie de fichiers nous paraît pouvoir être en partie pouvoir être réduite par des interfaces bien conçues ainsi que l’ont démontré les projet commerciaux mentionnés plus haut.

Vers où aller aujourd’hui. On pourrait bien sûr pour commencer essayer d’avancer avec les éditeurs libres et open source comme emacs ou vim qui restent encore très utilisés par les codeurs. Mais leur interface fait fuir beaucoup d’utilisateurs modernes et reste peu accessibles aux acteurs de l’édition numérique ou aux chercheurs des disciplines littéraires ou historiques. Depuis quelques années, de nouveaux éditeurs rédigés en JavaScript comme [Brackets](http://brackets.io) ou [Atom](https://atom.io) se sont très largement imposés en proposant des applications multiplateformes facilement personnalisables. C’est la raison pour laquelle nous pensons qu’il serait plus stratégique aujourd’hui d’investir les développements sur Atom dont la conception est particulièrement versatile, et dont le projet est désormais libre et open source. Surtout on peut largement s’appuyer sur les implémentations des processeurs XML pour créer un éditeur particulièrement efficace.

Les fonctionnalités que devraient remplir un éditeur XML natif moderne

- contrôle de la conformité
- validation contre un schéma
- saisie contextuelle d’après un schéma ([RelaxNG](http://relaxng.org), [W3C XML Schema](https://www.w3.org/XML/Schema) et pourquoi pas nativement ODD)
- refactoring d’éléments
- visualisation et navigation dans l’arbre
- recherches XPath
- mode auteur
- raccourcis clavier pour l’édition
- transformations XSLT (conversions vers d’autres formats)
- sélection schéma, etc.

Un soin tout particulier devrait être accordé au mode d’édition sans balise en vue d’un utilisateur type qui serait un auteur d’édition critique ou un historien voulant annoter des sources historiques.

Il y a donc beaucoup de travail. Mais la possibilité de tirer partie du framework offert par Atom est une véritable occasion pour sortir de l’ornière.



[1] Ce travail a fait l’objet de plusieurs publications et présentations publiques, notamment : Emmanuel Château, Marcello Vitali-Rosati, « Repenser la chaîne éditoriale numérique pour les revues savantes en sciences humaines », dans Congrès annuel de la Société canadienne des humanités numériques, Calgary, 28 au 3 juin 2016.



