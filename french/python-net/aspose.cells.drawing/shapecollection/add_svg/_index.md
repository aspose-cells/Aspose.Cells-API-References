---
title: add_svg méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 300
url: /fr/python-net/aspose.cells.drawing/shapecollection/add_svg/
is_root: false
---
##  add_svg(upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data) {#int-int-int-int-int-int-bytes-bytes}
Ajoute une image svg.


###  Retour




```python
def add_svg(self, upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| upper_left_row | int | Index de ligne en haut à gauche.|
| top | int | Représente le décalage vertical de la forme par rapport à sa ligne de gauche, en unité de pixel.|
| upper_left_column | int | Index de la colonne en haut à gauche.|
| left | int | Décalage horizontal de la forme par rapport à sa colonne de gauche, en pixels.|
| height | int | La hauteur de la forme, en unité de pixel.|
| width | int | La largeur de la forme, en unité de pixel.|
| svg_data | bytes | Les données d'image svg.|
| compatible_image_data | bytes |Conversion des données d'image à partir de svg afin d'être compatible avec Excel 2016 ou versions antérieures.|

###  Exemple

```python
from aspose import pycore

#  add a svg
with open("image.svg", "rb") as fs:
    len = pycore.cast(int, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
    picture = shapes.add_svg(4, 0, 5, 0, -1, -1, imageData, None)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/fr/python-net/aspose.cells.drawing/shapecollection)
