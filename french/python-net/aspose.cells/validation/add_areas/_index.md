---
title: add_areas méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells/validation/add_areas/
is_root: false
---
##  add_areas(areas, check_intersection, check_edge) {#list-bool-bool}
Applique la validation à des zones données.



```python
def add_areas(self, areas, check_intersection, check_edge):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| areas | list | Les zones.|
| check_intersection | bool | Que ce soit vérifier l'intersection de la zone donnée avec les zones de validations existantes.<br/>Si une validation a été appliquée dans une zone donnée (ou une partie de celle-ci),<br/>alors la validation existante doit d'abord être supprimée de la zone donnée.<br/>Sinon, une corruption peut être causée pour les validations générées.<br/>Si l'utilisateur est sûr que toutes les zones ajoutées ne se croisent avec aucune zone existante,<br/> ce paramètre peut être défini sur false pour des raisons de performances.|
| check_edge | bool | Que ce soit vérifier le bord des zones appliquées de cette validation.<br/>Les paramètres internes de la validation dépendent de la plage supérieure gauche de ses plages appliquées,<br/>donc si l'une des zones données deviendra la nouvelle en haut à gauche des plages appliquées,<br/>les paramètres internes doivent être modifiés et reconstruits, sinon un résultat inattendu peut être causé.<br/>Si l'utilisateur est sûr qu'aucune de ces zones ajoutées n'est en haut à gauche,<br/> ce paramètre peut être défini sur false pour des raisons de performances.|
###  Remarques

Dans cette méthode, nous supprimerons toutes les anciennes validations dans une zone donnée.
Pour la plage supérieure gauche appliquée de Validation, premièrement, sa StartRow est la plus petite,
deuxièmement, sa StartColumn est la plus petite de ces zones qui ont la même StartRow la plus petite.


###  Voir également
* module [aspose.cells](../../)
* classe [Validation](/cells/fr/python-net/aspose.cells/validation)
