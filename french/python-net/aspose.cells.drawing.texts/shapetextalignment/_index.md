---
title: ShapeTextAlignment classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 80
url: /fr/python-net/aspose.cells.drawing.texts/shapetextalignment/
is_root: false
---
##  ShapeTextAlignment classe
Représente le paramètre d'alignement du texte de la forme ;



Le type ShapeTextAlignment expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [is_text_wrapped](/cells/fr/python-net/aspose.cells.drawing.texts/shapetextalignment/is_text_wrapped) | Obtient et définit le type de texte enveloppé de la forme qui contient du texte.|
| [rotate_text_with_shape](/cells/fr/python-net/aspose.cells.drawing.texts/shapetextalignment/rotate_text_with_shape) | Indique s'il faut faire pivoter le texte avec la forme.|
| [text_vertical_overflow](/cells/fr/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_overflow) | Obtient et définit le type de débordement vertical du texte de la zone de texte.|
| [text_horizontal_overflow](/cells/fr/python-net/aspose.cells.drawing.texts/shapetextalignment/text_horizontal_overflow) | Obtient et définit le type de débordement horizontal du texte de la zone de texte.|
| [rotation_angle](/cells/fr/python-net/aspose.cells.drawing.texts/shapetextalignment/rotation_angle) | Obtient et définit la rotation de la forme.|
| [text_vertical_type](/cells/fr/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_type) | Obtient et définit la direction du texte.|
| [auto_size](/cells/fr/python-net/aspose.cells.drawing.texts/shapetextalignment/auto_size) |Indique si la taille de la forme est ajustée automatiquement en fonction de son contenu.|
| [text_shape_type](/cells/fr/python-net/aspose.cells.drawing.texts/shapetextalignment/text_shape_type) | Obtient et définit le type de transformation du texte.|
| [top_margin_pt](/cells/fr/python-net/aspose.cells.drawing.texts/shapetextalignment/top_margin_pt) | Renvoie la marge supérieure en unité de points|
| [bottom_margin_pt](/cells/fr/python-net/aspose.cells.drawing.texts/shapetextalignment/bottom_margin_pt) | Renvoie la marge inférieure en unité de points|
| [left_margin_pt](/cells/fr/python-net/aspose.cells.drawing.texts/shapetextalignment/left_margin_pt) | Renvoie la marge de gauche en unité de Points|
| [right_margin_pt](/cells/fr/python-net/aspose.cells.drawing.texts/shapetextalignment/right_margin_pt) | Renvoie la marge de droite en unité de Points|
| [is_auto_margin](/cells/fr/python-net/aspose.cells.drawing.texts/shapetextalignment/is_auto_margin) | Indique si la marge du cadre de texte est automatique.|
| [number_of_columns](/cells/fr/python-net/aspose.cells.drawing.texts/shapetextalignment/number_of_columns) | Obtient et définit le nombre de colonnes de texte dans le rectangle englobant.|



###  Exemple

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
shape = workbook.worksheets[0].shapes.add_rectangle(1, 0, 1, 0, 50, 100)
shapeTextAlignment = shape.text_body.text_alignment

```

###  Voir également
* module [aspose.cells.drawing.texts](..)
