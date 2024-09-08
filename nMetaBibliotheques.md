---
tags: bibliothèques
since: 2019-04-01
versions: 
  - 2.0 (2024-05-31)
---

# Méta-bibliothèques

Au cours d’une réunion du Café des savoirs libres, j’ai fait part d’une idée qui me tient à cœur depuis quelques années. C’est un projet que j’ai déjà eu l’occasion de rapidement esquissé auprès de la direction de ma bibliothèque, mais sans réel succès jusqu’à présent. Pourtant, il me paraît d’autant plus pertinent aujourd’hui que je réside en Amérique du Nord. En effet, à l’heure de la numérisation patrimoniale de masse, on peut légitiment se poser la question du rôle des bibliothèques Nord-Américaines alors même que leurs collections, hormis certains secteurs spécialisés comme ici les Canadiana, sont souvent moins riches que celles de leurs homologues européennes. 

Il me semble intéressant de concevoir des métabibliothèques numériques qui tirent largement parti du travail de numérisation déjà effectué en organisant l’accès au contenu et aux ressources à travers sur des sujets choisis. Un tel projet s’inscrit directement dans une logique bibliothécaire, c’est la raison pour laquelle j’ai suggéré à Marie Martel cette idée pour l’atelier *Publishing sphere* avec des thématiques telles que la lecture publique et l’architecture sur lequel je travaille déjà dans cet esprit depuis quelques années.

- Sélectionner les contenus dans une logique bibliothécaire
- Organiser des accès thématiques spécialisés en éditorialisant ces contenus
- Offrir un accès enrichi au texte grâce à des chaînes de numérisation automatisée (OCR, conversion TEI, réindexation)

Le projet est directement inspiré des [Living Book of History](http://livingbooksabouthistory.ch) lancés en 2016.

Sur le sujet, voir Parkinson, Isabelle. 2018. « Can Curation Free the Anthology? Giorgio Agamben’s Apparatus and Against Expression: An Anthology of Conceptual Writing ». *Postmodern Culture* 28 (2). <https://doi.org/10.1353/pmc.2018.0013>.

Notion de collections https://peterwebster.me/2018/02/20/the-edited-collection-pasts-present-and-future/

## Questions à travailler

Comment penser une monté en charge graduelle du projet pour ne pas attendre que des ressources soient immédiatement disponibles pour sa réalisation ? Faire une preuve de concept, sélectionner des approches très low tech ?

Comment rester pertinent alors que les fonctionnalités offertes par les bibliothèques numériques vont sans doute s’améliorer pour la recherche ?

Une soutenabilité économique est-elle envisageable ? Commercialisation de formats détachables, etc.

Penser la valeur ajoutée de la collection au-delà du corpus ? Liens possibles entre les items, etc.

Travailler la question de la granularité pour les textes multiples, l’extraction des images, mais aussi la fédération de contenus grâce à l’indexation

Comment rendre le corpus adapté aux traitements automatiques permis par l’IA ? Où la plateforme doit-elle arbitrer entre la curation et le traitement manuels et le traitement automatique ? 

Travailler le contexte de lecture et les emplois scientifiques. Citabilité, annotation, indexation, modes de lectures, importatation/exportation, etc.

Dans quelle mesure l’API textuelle DTS est adaptée à la publication du corpus.

## Fonctionnalités

Bibliothèques numériques génériques conçues dans un contexte de numérisation industrielle. Ne supprime pas le besoin de collections spécialisées, structurées et organisées avec soin.

Pb de la gratuité et du soin. Nécessité de trouver des modèles pour garantir la curation des contenus et la responsabilité.

### Fonctionnalités de recherche avancée

Fonctionnalités de recherche avancée par troncature, stemming et suite d’opérateur bolléens.

### Outils sociaux

Suivre des sujets, des personnes ou des organisations. Création de portails personnalisés, recevoir des alertes.

### Contenus enrichis

Enrichissement des données et retraitement. 

Fonctionnalités d’exportation.

Production du plein texte : océrisation qualitative, etc.

Réindexation spécialisée des contenus

### Contributions

Fonctionnalités de contribution, charger des documents dans la communauté

Création de fonctionnalités de lecture sociale

Carnet de citations, Partage citations ?

### Intégration

Intégration avec les systèmes de découvertes bibliothécaires (Summon, EBSCO Discovery Service (EDS), and Primo).

Citablité et exposition des métadonnées.

APIs

### Page d’accueil

Moteur de recherche simple et avancé, avec mise en avant de tags.

Tableau de bord : Provenance (nb d’organisations/organizations), Items (nb de publications/publications), Sujets (nb de sujets/topics).

Mise en avant, d’organisations de publications (lien vers tous)

Listes mise en avant

Sujets mis en avant

## Exemples inspirants

### Canada Commons

https://canadacommons.ca

Service commercial d’agrégation et de réorganisation de ressources en libre accès développé par Coherent Digital.

### Living Books of History (2016)

http://livingbooksabouthistory.ch

>Living Books about History represent a new  form of digital anthology. They present short essays on current topics  of scholarly interest accompanied by selected contributions that are  freely available online. 
>
>The project is  testing a new form of scholarly publication and aims to draw attention  to the potentials of open access by rediscovering and reusing scholarly  texts and sources.

Le projet est inspiré des [Living Books about Life](https://www.livingbooksaboutlife.org/), une série de publications initiée par Coventry University en 2011 sous la direction de Gary Hall.

### Living Books about Life (2011)

https://www.livingbooksaboutlife.org

> Funded by the Joint Information Systems Committee (JISC), and published by Open Humanities Press (OHP) (https://openhumanitiespress.org), Living Books About Life is a series of curated, open access books about life -- with life understood both philosophically and biologically --  which provide a bridge between the humanities and the sciences. Produced by a globally-distributed network of writers and editors, the books in  the series repackage existing open access science research by clustering it around selected topics whose unifying theme is life: e.g., air,  agriculture, bioethics, cosmetic surgery, electronic waste, energy,  neurology and pharmacology.
>
> By creating twenty one ‘living books about life’ in just seven months,  the series represents an exciting new model for publishing, in a  sustainable, low-cost manner, many more such books in the future. These  books can be freely shared with other academic and non-academic  institutions and individuals. Taken together, they constitute an  engaging interdisciplinary resource for researching and teaching  relevant science issues across the humanities, a resource that is  capable of enhancing the intellectual and pedagogic experience of  working with open access materials.
>
> All the books in the series are themselves ‘living’, in the sense that  they are open to ongoing collaborative processes of writing, editing,  updating, remixing and commenting by readers. As well as repackaging  open access science research -- along with interactive maps,  visualisations, podcasts and audio-visual material -- into a series of  books, Living Books About Life is thus engaged in rethinking ‘the book’  itself as a living, collaborative endeavour in the age of open science,  open education, open data and e-book readers such as Kindle and the  iPad.
>
> Living Books About Life is a collaboration between Open Humanities  Press and three academic institutions: Coventry University, Goldsmiths,  University of London, and the University of Kent.

### Jisedai Reader: A UX-centered Approach for Digital Social Reading of Historical Japanese Books

Dimension sociale, etc. mais implique gestion comptes utilisateurs.
