---
title: add_area méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells/validation/add_area/
is_root: false
---
##  add_area(cell_area) {#CellArea}
Applique la validation à la zone.



```python
def add_area(self, cell_area):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| cell_area | [CellArea](/cells/fr/python-net/aspose.cells/cellarea) | La zone.|
###  Remarques

Il équivaut à utiliser [Validation.add_area(cell_area)](/cells/fr/python-net/aspose.cells/validation/add_area)
avec vérification des intersections et des bords.

##  add_area(cell_area, check_intersection, check_edge) {#CellArea-bool-bool}
Applique la validation à la zone.



```python
def add_area(self, cell_area, check_intersection, check_edge):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| cell_area | [CellArea](/cells/fr/python-net/aspose.cells/cellarea) | La zone.|
| check_intersection | bool | Que ce soit vérifier l'intersection de la zone donnée avec les zones de validations existantes.<br/>Si une validation a été appliquée dans une zone donnée (ou une partie de celle-ci),<br/>alors la validation existante doit d'abord être supprimée de la zone donnée.<br/>Sinon, une corruption peut être causée par les validations générées.<br/>Si l'utilisateur est sûr que la zone ajoutée ne croise aucune zone existante,<br/> Ce paramètre peut être défini sur false pour des raisons de performances.|
| check_edge | bool | Que ce soit vérifier le bord des zones appliquées de cette validation.<br/>Les paramètres internes de la validation dépendent de la plage supérieure gauche de ses plages appliquées,<br/>donc si la zone donnée deviendra la nouvelle en haut à gauche des plages appliquées,<br/>les paramètres internes doivent être modifiés et reconstruits, sinon des résultats inattendus peuvent être provoqués.<br/>Si l'utilisateur est sûr que la zone ajoutée n'est pas celle en haut à gauche,<br/> Ce paramètre peut être défini sur false pour des raisons de performances.|
###  Remarques

Dans cette méthode, nous supprimerons toutes les anciennes validations dans une zone donnée.
Pour la plage supérieure gauche appliquée de Validation, premièrement, sa StartRow est la plus petite,
deuxièmement, sa StartColumn est la plus petite de ces zones qui ont la même StartRow la plus petite.


###  Voir également
* module [aspose.cells](../../)
* classe [Validation](/cells/fr/python-net/aspose.cells/validation)
