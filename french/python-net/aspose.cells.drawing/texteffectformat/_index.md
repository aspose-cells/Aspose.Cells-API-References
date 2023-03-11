---
title: TextEffectFormat classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 700
url: /fr/python-net/aspose.cells.drawing/texteffectformat/
is_root: false
---
##  TextEffectFormat classe
Contient des propriétés et des méthodes qui s'appliquent aux objets WordArt.



Le type TextEffectFormat expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [text](/cells/fr/python-net/aspose.cells.drawing/texteffectformat/text) | Le texte dans le WordArt.|
| [font_name](/cells/fr/python-net/aspose.cells.drawing/texteffectformat/font_name) | Le nom de la police utilisée dans le WordArt.|
| [font_bold](/cells/fr/python-net/aspose.cells.drawing/texteffectformat/font_bold) | Indique si la police est en gras.|
| [font_italic](/cells/fr/python-net/aspose.cells.drawing/texteffectformat/font_italic) | Indique si la police est en italique.|
| [rotated_chars](/cells/fr/python-net/aspose.cells.drawing/texteffectformat/rotated_chars) | Si true, les caractères du WordArt spécifié pivotent de 90 degrés par rapport à la forme de délimitation du WordArt.|
| [font_size](/cells/fr/python-net/aspose.cells.drawing/texteffectformat/font_size) | La taille (en points) de la police utilisée dans le WordArt.|
| [preset_shape](/cells/fr/python-net/aspose.cells.drawing/texteffectformat/preset_shape) | Obtient et définit le type de forme prédéfini.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [set_text_effect(effect)](/cells/fr/python-net/aspose.cells.drawing/texteffectformat/set_text_effect/#MsoPresetTextEffect) | Définit l'effet de texte prédéfini.|



###  Exemple

```python
from aspose.cells import Workbook
from aspose.cells.drawing import MsoPresetTextEffect

# Instantiating a Workbook object
workbook = Workbook()
shapes = workbook.worksheets[0].shapes
shapes.add_text_effect(MsoPresetTextEffect.TEXT_EFFECT1, "Aspose", "Arial", 30, False, False, 0, 0, 0, 0, 100, 200)
textEffectFormat = shapes[0].text_effect
textEffectFormat.set_text_effect(MsoPresetTextEffect.TEXT_EFFECT10)
workbook.save("Book1.xls")

```

###  Voir également
* module [aspose.cells.drawing](..)
