---
title: inner_height propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 150
url: /fr/python-net/aspose.cells.charts/plotarea/inner_height/
is_root: false
---
##  inner_height propriété

Obtient ou définit la hauteur de la zone de tracé en unités de 1/4000 de la zone de graphique.

###  Remarques

La boîte englobante de la zone de tracé comprend la zone de tracé, les graduations (étiquettes de graduation) et une petite bordure autour des graduations.
Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.


 Le**X** , **Y** , **Largeur** et**Hauteur** de**Zone de tracé** représente la surface de la parcelle
 boîte englobante qui comprend la zone de tracé, les graduations (étiquettes de graduation) et une petite bordure autour des graduations.
 Si vous voulez obtenir la taille réelle de la zone de tracé, vous devez appeler**IntérieurX** , **IntérieurY** , **Largeurintérieure** et
**Hauteurintérieure** propriétés.


Pour Excel 2007 ou ultérieur, la valeur par défaut est zéro. vous devez appeler obtenir la valeur après avoir appelé Chart.Calculate().
###  Définition:
```python
@property
def inner_height(self):
    ...
@inner_height.setter
def inner_height(self, value):
    ...
```

###  Voir également
* module [aspose.cells.charts](../../)
* classe [PlotArea](/cells/fr/python-net/aspose.cells.charts/plotarea)
