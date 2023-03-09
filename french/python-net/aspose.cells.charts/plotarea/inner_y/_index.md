---
title: inner_y propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 180
url: /fr/python-net/aspose.cells.charts/plotarea/inner_y/
is_root: false
---
##  inner_y propriété

Obtient ou obtient la coordonnée x du coin supérieur supérieur de la zone de tracé en unités de 1/4000 de la zone de graphique.

###  Remarques

La boîte englobante de la zone de tracé comprend la zone de tracé, les graduations (étiquettes de graduation) et une petite bordure autour des graduations.
 Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.


 Le**X** , **Y** , **Largeur** et**Hauteur** de**Superficie du terrain** représente la surface de la parcelle
 Une zone de délimitation qui inclut la zone de tracé, des graduations (étiquettes de graduation) et une petite bordure autour des graduations.
 Si vous voulez obtenir la taille réelle de la zone de tracé, vous devez appeler**X intérieur** , **Y intérieur** , **Largeur intérieure** et
**Hauteur intérieure** propriétés.


Pour Excel 2007 ou ultérieur, la valeur par défaut est zéro.
###  Définition:
```python
@property
def inner_y(self):
    ...
@inner_y.setter
def inner_y(self, value):
    ...
```

###  Voir également
* module [aspose.cells.charts](../../)
* classe [PlotArea](/cells/fr/python-net/aspose.cells.charts/plotarea)
