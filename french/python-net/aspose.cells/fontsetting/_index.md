---
title: FontSetting classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 670
url: /fr/python-net/aspose.cells/fontsetting/
is_root: false
---
##  FontSetting classe
Représente une plage de caractères dans le texte de la cellule.



Le type FontSetting expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [FontSetting(start_index, length, sheets)](/cells/fr/python-net/aspose.cells/fontsetting/__init__/#int-int-WorksheetCollection) |  |


###  Propriétés
| Propriété| Description|
| :- | :- |
| [type](/cells/fr/python-net/aspose.cells/fontsetting/type) | Obtient le type de nœud de texte.|
| [start_index](/cells/fr/python-net/aspose.cells/fontsetting/start_index) | Obtient l'index de début des caractères.|
| [length](/cells/fr/python-net/aspose.cells/fontsetting/length) |Obtient la longueur des caractères.|
| [font](/cells/fr/python-net/aspose.cells/fontsetting/font) | Renvoie la police de cet objet.|
| [text_options](/cells/fr/python-net/aspose.cells/fontsetting/text_options) | Renvoie les options de texte.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [set_word_art_style(style)](/cells/fr/python-net/aspose.cells/fontsetting/set_word_art_style/#aspose.cells.drawing.PresetWordArtStyle) | Définit le style WordArt prédéfini.|



###  Exemples

```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Accessing the "A1" cell from the worksheet
cell = worksheet.cells.get("A1")
# Adding some value to the "A1" cell
cell.put_value("Visit Aspose!")
# getting charactor
charactor = cell.characters(6, 7)
# Setting the font of selected characters to bold
charactor.font.is_bold = True
# Setting the font color of selected characters to blue
charactor.font.color = Color.blue
# Saving the Excel file
workbook.save("book1.xls")

```

###  Voir également
* module [aspose.cells](..)
