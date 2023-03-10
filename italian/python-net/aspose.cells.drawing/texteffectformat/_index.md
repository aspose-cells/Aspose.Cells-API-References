---
title: classe TextEffectFormat
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 700
url: /it/python-net/aspose.cells.drawing/texteffectformat/
is_root: false
---
##  classe TextEffectFormat
Contiene proprietà e metodi che si applicano agli oggetti WordArt.



Il tipo TextEffectFormat espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [text](/cells/it/python-net/aspose.cells.drawing/texteffectformat/text) | Il testo nel WordArt.|
| [font_name](/cells/it/python-net/aspose.cells.drawing/texteffectformat/font_name) | Il nome del carattere utilizzato nell'oggetto WordArt.|
| [font_bold](/cells/it/python-net/aspose.cells.drawing/texteffectformat/font_bold) | Indica se il carattere è in grassetto.|
| [font_italic](/cells/it/python-net/aspose.cells.drawing/texteffectformat/font_italic) | Indica se il carattere è corsivo.|
| [rotated_chars](/cells/it/python-net/aspose.cells.drawing/texteffectformat/rotated_chars) | Se true, i caratteri nell'oggetto WordArt specificato vengono ruotati di 90 gradi rispetto alla forma di delimitazione dell'oggetto WordArt.|
| [font_size](/cells/it/python-net/aspose.cells.drawing/texteffectformat/font_size) | La dimensione (in punti) del carattere utilizzato nell'oggetto WordArt.|
| [preset_shape](/cells/it/python-net/aspose.cells.drawing/texteffectformat/preset_shape) | Ottiene e imposta il tipo di forma preimpostato.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [set_text_effect(effect)](/cells/it/python-net/aspose.cells.drawing/texteffectformat/set_text_effect/#MsoPresetTextEffect) | Imposta l'effetto di testo preimpostato.|



###  Esempio

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

###  Guarda anche
* modulo [aspose.cells.drawing](..)
