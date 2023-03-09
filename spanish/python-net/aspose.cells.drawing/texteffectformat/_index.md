---
title: TextEffectFormat clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 700
url: /es/python-net/aspose.cells.drawing/texteffectformat/
is_root: false
---
##  TextEffectFormat clase
Contiene propiedades y métodos que se aplican a los objetos de WordArt.



El tipo TextEffectFormat expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [text](/cells/es/python-net/aspose.cells.drawing/texteffectformat/text) | El texto en el WordArt.|
| [font_name](/cells/es/python-net/aspose.cells.drawing/texteffectformat/font_name) | El nombre de la fuente utilizada en WordArt.|
| [font_bold](/cells/es/python-net/aspose.cells.drawing/texteffectformat/font_bold) | Indica si la fuente está en negrita.|
| [font_italic](/cells/es/python-net/aspose.cells.drawing/texteffectformat/font_italic) | Indica si la fuente está en cursiva.|
| [rotated_chars](/cells/es/python-net/aspose.cells.drawing/texteffectformat/rotated_chars) | Si es verdadero, los caracteres del WordArt especificado se giran 90 grados en relación con la forma delimitadora del WordArt.|
| [font_size](/cells/es/python-net/aspose.cells.drawing/texteffectformat/font_size) | El tamaño (en puntos) de la fuente utilizada en WordArt.|
| [preset_shape](/cells/es/python-net/aspose.cells.drawing/texteffectformat/preset_shape) | Obtiene y establece el tipo de forma preestablecido.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [set_text_effect(effect)](/cells/es/python-net/aspose.cells.drawing/texteffectformat/set_text_effect/#MsoPresetTextEffect) | Establece el efecto de texto predeterminado.|



###  Ejemplos

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

###  Ver también
* módulo [aspose.cells.drawing](..)
