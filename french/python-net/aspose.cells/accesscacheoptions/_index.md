---
title: AccessCacheOptions dénombrement
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1740
url: /fr/python-net/aspose.cells/accesscacheoptions/
is_root: false
---
##  AccessCacheOptions dénombrement
Options de cache pour l'accès aux données. Peut être combiné avec l'opérateur | pour plusieurs options ensemble.



Le type AccessCacheOptions expose les membres suivants :

###  Des champs
| Champ| Description|
| :- | :- |
| NONE | Pas de cache pour tout accès aux données.|
| ALL | Appliquez toutes les optimisations possibles pour tous les types d'accès aux données dans le classeur.<br/> Tous les paramètres et données ne doivent pas être modifiés pendant l'accès optimisé.|
| POSITION_AND_SIZE | Appliquez une optimisation possible pour obtenir la position et la taille de l'objet (tel que la forme).<br/>Les paramètres de hauteur de ligne et de largeur de colonne ne doivent pas être modifiés pendant l'accès optimisé.|
| CELLS_DATA | Appliquez une optimisation possible pour obtenir les valeurs des cellules.<br/>Les données Cells (données et paramètres de Cell, ligne) ne doivent pas être modifiées pendant<br/>l'accès optimisé, aucun nouvel objet Cell/Row ne doit être créé non plus (tel que<br/> par [[indexer]](/cells/python-net/aspose.cells/cells/__getitem__/)).|
| CELL_DISPLAY | Appliquer une optimisation possible pour obtenir des résultats liés à l'affichage de<br/>cellules ([Cell.display_string_value](/cells/fr/python-net/aspose.cells/cell#display_string_value), [Cell.get_style()](/cells/fr/python-net/aspose.cells/cell/get_style), [Cell.get_display_style()](/cells/fr/python-net/aspose.cells/cell/get_display_style), etc.).<br/>Cells données et objets liés au style (Cell/styles de ligne/colonne, largeur de colonne, etc.) ne doivent pas être modifiés<br/> lors de l'accès optimisé.|
| GET_FORMULA | Appliquer une optimisation possible pour obtenir des formules.<br/>Toutes les données et tous les paramètres susceptibles d'affecter l'expression de la formule (nom de la feuille de calcul, texte du nom,<br/> colonnes de la table, etc.) ne doivent pas être modifiés lors de l'accès optimisé.|
| SET_FORMULA | Appliquer les optimisations possibles pour définir les formules.<br/>Toutes les données et tous les paramètres susceptibles d'affecter l'expression de la formule (nom de la feuille de calcul, texte du nom,<br/> colonnes de la table, etc.) ne doivent pas être modifiés lors de l'accès optimisé.|
| CALCULATE_FORMULA |Appliquer une optimisation possible pour le calcul des formules.<br/>Les données Cells ne doivent pas être modifiées lors de l'accès optimisé, aucun nouvel objet (Cell, Row, etc.)<br/> doit être créé soit (comme par [[indexer]](/cells/python-net/aspose.cells/cells/__getitem__/)).|
| CONDITIONAL_FORMATTING | Appliquez une optimisation possible pour obtenir les résultats de mise en forme des mises en forme conditionnelles.<br/>Toutes les données et tous les paramètres susceptibles d'affecter le résultat du formatage conditionnel (paramètres de<br/> mises en forme conditionnelles, valeurs de cellules dépendantes, etc.) ne doivent pas être modifiées pendant l'accès optimisé.|
| VALIDATION | Appliquer une optimisation possible pour obtenir des résultats de validation.<br/>Toutes les données et paramètres pouvant affecter le résultat de la validation (paramètres de la validation,<br/> les valeurs des cellules dépendantes, etc.) ne doivent pas être modifiées pendant l'accès optimisé.|



###  Remarques

Pour certaines fonctionnalités, l'accès à de grands ensembles de données nécessite de nombreuses opérations répétées et compliquées
telles que la recherche, le calcul, etc. et ces opérations prendront beaucoup de temps supplémentaire.
Pour les situations courantes, toutes les données dépendantes restent inchangées pendant l'accès, de sorte que certains caches peuvent être créés et utilisés pour
améliorer les performances d'accès.
À cette fin, nous fournissons ce API afin que l'utilisateur puisse spécifier le type d'accès aux données dont il a besoin
à optimiser par un éventuel mécanisme de mise en cache.


Veuillez noter que pour différentes options, différents ensembles de données peuvent devoir être "en lecture seule".
Et les performances d'accès aux données dépendent de nombreux aspects, l'utilisation du mécanisme de mise en cache
ne garantit pas que les performances seront améliorées.
comme l'ensemble de données auquel accéder est petit, l'utilisation du cache peut prendre encore plus de temps car
la mise en cache elle-même nécessite également un certain temps supplémentaire.

###  Voir également
* module [aspose.cells](..)
