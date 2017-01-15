---
author: Emmanuel Château-Dutier
since: 2017-01-14
tags: topic modeling, textométrie
---

# Le topic modeling, une stratégie adaptée pour notre recherche ?

Le *Topic modeling* est une approche textométrique introduite par [David Blei en 2003](http://www.cs.princeton.edu/~blei/papers/BleiNgJordan2003.pdf) qui consiste à analyser les contextes lexicaux de façon à offrir une représentation du contenu du texte. De ce point de vue, il s’agit d’une approche de lecture distante qui cherche à rendre compte du contenu sémantique d’un corpus. C’est une technique puissante, facile à utiliser mais difficile à interpréter. Elle peut être couplée avec des procédés de visualisation, par exemple en utilisant la librairie JavaScript [d3.js](https://d3js.org).

## Les technologiques d’analyse sémantique latente

Le topic modeling repose sur l’utilisation des approches dites de Latent Semantic Analysis (LSA) et de Latent Dirichlit Allocation (LDA). Fondamentalement, ces méthodes reposent sur l’utilisation de matrices [tf–idf (term frequency–inverse document frequency)](https://fr.wikipedia.org/wiki/TF-IDF) qui consistent à pondérer l’importance d’un mot dans un document relativement à une collection ou un corpus par l’utilisation de méthodes statistiques. Pour chacun des documents, on détermine une liste de mots classées par leur fréquence. Le tf-idf permet de fournir un score en fonction de leur spécificité pour un document donné par rapport au corpus d’ensemble.

L’[analyse sémantique latente](Latent Semantic Analy…) (LSA de *Latent Semantic Analysis* en anglais) utilise notamment des scores tf-idf dans une matrice de termes large destinée notamment à la catégorisation des textes. Elle permet d’établir des relations entre un ensemble de documents et les termes que ceux-ci contiennent, en construisant des « concepts » liés aux documents et aux termes. Chacun des termes du corpus donne lieu à une évaluation de son occurence dans chaque document. Souvent les termes sont ramenés à leurs radicaux. Cette matrice comporte nécessairement de nombreuses valeurs nulles car peu de documents utilisent probablement peu de mots relatifs au corpus général. Au sein de cette matrice, l’analyse sémantique latente emploie une [décomposition en valeurs singulières](https://fr.wikipedia.org/wiki/Décomposition_en_valeurs_singulières) pour déterminer quel mot est en rapport avec tel autre. Pour simplifier, plus des mots sont employés concurremment dans un document, plus ils seront considérés en rapport les uns avec les autres.

cf. http://webapp1.dlib.indiana.edu/newton/lsa/

Cette technique fut d’abord significativement améliorée par Puzicha et Hofmann en 1999 par l’introduction reposant sur l’utilisation de l’algèbre linéaire pour obtenir un modèle probabiliste désigné l’[analyse sémantique latente probabiliste](http://en.wikipedia.org/wiki/Probabilistic_latent_semantic_analysis) (*probabilistic latent semantic analysis* (pLSA) en anglais). Celle-ci consiste à ajouter un niveau d’analyse qui serait les sujets ou les domaines (*topics*). [Blei et ses collègues](http://www.cs.princeton.edu/~blei/papers/BleiNgJordan2003.pdf) ont considérablement fait évolué cette idée en en un modèle génératif probabiliste appelé l’[allocation de Dirichlet latente](https://fr.wikipedia.org/wiki/Allocation_de_Dirichlet_latente) (*Latent Dirichlet Allocation* (LDA) en anglais). Avec cette méthode, les documents deviennent des ensemble de *topics* qui peuvent être étudiés. Même si ceux-ci n’existent-pas, ils offrent des représentations du contenu sémantique des documents, ce qui permet de les classifier.

Si l’on peut générer des documents à partir de ce modèle, le processus peut également être employé pour inférer qu’un document se rattache à un modèle déjà dégagé. D’autre part, ces modèles peuvent être étendus pour rendre compte de changements et de variations temporels. Ted Underwood et Lisa Rhode avancent que les historiens peuvent les appréhender, avec les précautions afférentes, comme des discours.

## Le topic modeling pour l’analyse du discours architectural

Il n’est pas évident que cette approche soit adaptée pour analyser la formation de la critique architecturale. Au-delà de l’évidente proximité terminologique des textes que nous sommes conduits à étudier, c’est plutôt la structure de l’argumentation et la divergence des avis qui nous intéresse. Il faudrait évaluer dans quelle mesure ce type d’analyse prend en charge la simple négation et l’expression du dissensus dans un même domaine.

Le topic modeling présente l’avantage de proposer un accès à la signification du texte sans le recours à une annotation lisible par la machine. Il présente également le potentiel de pouvoir aborder des évolutions longitudinales. Mais il n’est pas certain que l’approche probabiliste présente un niveau de preuve suffisant en histoire car elle suppose de formuler des jugements qui définissent largement la nature des résultats (choix des mots vides, nombre de topics sélectionnés, portée de la collection). Aussi les modèles produits sont construits et parfois difficiles à expliquer. Des approches plus directes comme la comparaison de corpus peuvent donc permettre de répondre de façon à la fois plus directe et plus transparente – et donc convaincante – à certaines questions. Enfin, ces méthodes sont relativement consommatrices de ressources computationnelles car elles impliquent la construction de variables pour chacun des mots du corpus.

Plusieurs évaluations pourraient être conduites

- identifier des dissensus et les caractérisés avec cette méthode
- tester jusqu’où le modèle permet de rendre compte dans un même domaine des distinctions de point de vue architectural
- évaluer la pertinence du modèle pour évaluer les changements temporels dans les références architecturales, la formulation des énoncés, et les jugements de goût

## Tutoriaux

- Shawn Graham, Scott Weingart et Ian Miligan. Getting Started with Topic Modeling and MALLET. The Programming Historian, 2 septembre 2012. http://programminghistorian.org/lessons/topic-modeling-and-mallet
- Underwood, Ted. "Seven ways humanists are using computers to understand text." The Stone and the Shell, 4 juin 2015. http://tedunderwood.com/2015/06/04/seven-ways-humanists-are-using-computers-to-understand-text/
- Underwood, Ted. "Topic modeling made just simple enough." The Stone and the Shell, 7 avril 2012. https://tedunderwood.com/2012/04/07/topic-modeling-made-just-simple-enough/

## Outils

Mallet, http://mallet.cs.umass.edu

## Sources

- Scott Weingart. « Topic Modeling and Network Analysis. » the scottbot irregular, 15 novembre 2011. <http://www.scottbot.net/HIAL/index.html@p=221.html>

- ​

  ​

