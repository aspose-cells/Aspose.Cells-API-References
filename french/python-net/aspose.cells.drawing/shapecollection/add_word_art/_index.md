---
title: add_word_art méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 350
url: /fr/python-net/aspose.cells.drawing/shapecollection/add_word_art/
is_root: false
---
##  add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width) {#PresetWordArtStyle-str-int-int-int-int-int-int}
Ajoute un WordArt prédéfini depuis Excel 2007.s


###  Retour




```python
def add_word_art(self, style, text, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| style | [PresetWordArtStyle](/cells/fr/python-net/aspose.cells.drawing/presetwordartstyle) | Le style WordArt prédéfini.|
| text | str | Le texte.|
| upper_left_row | int | Index de ligne en haut à gauche.|
| top | int | Représente le décalage vertical de la forme par rapport à sa ligne de gauche, en unité de pixel.|
| upper_left_column | int | Index de la colonne en haut à gauche.|
| left | int |Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pixel.|
| height | int | Représente la hauteur de la forme, en unités de pixels.|
| width | int | Représente la largeur de la forme, en unités de pixels.|

###  Exemples

```python
from aspose.cells.drawing import PresetWordArtStyle

# add a WordArt
wordArt2 = shapes.add_word_art(PresetWordArtStyle.WORD_ART_STYLE1, "WordArt", 3, 0, 3, 0, 50, 200)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/fr/python-net/aspose.cells.drawing/shapecollection)
