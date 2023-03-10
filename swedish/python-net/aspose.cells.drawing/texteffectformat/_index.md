---
title: TextEffectFormat klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 700
url: /sv/python-net/aspose.cells.drawing/texteffectformat/
is_root: false
---
##  TextEffectFormat klass
Innehåller egenskaper och metoder som gäller för WordArt-objekt.



Typen TextEffectFormat avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [text](/cells/sv/python-net/aspose.cells.drawing/texteffectformat/text) | Texten i WordArt.|
| [font_name](/cells/sv/python-net/aspose.cells.drawing/texteffectformat/font_name) | Namnet på teckensnittet som används i WordArt.|
| [font_bold](/cells/sv/python-net/aspose.cells.drawing/texteffectformat/font_bold) | Anger om teckensnittet är fetstilt.|
| [font_italic](/cells/sv/python-net/aspose.cells.drawing/texteffectformat/font_italic) | Anger om teckensnittet är kursivt.|
| [rotated_chars](/cells/sv/python-net/aspose.cells.drawing/texteffectformat/rotated_chars) | Om det är sant, roteras tecken i den angivna WordArt 90 grader i förhållande till WordArts avgränsande form.|
| [font_size](/cells/sv/python-net/aspose.cells.drawing/texteffectformat/font_size) | Storleken (i punkter) på teckensnittet som används i WordArt.|
| [preset_shape](/cells/sv/python-net/aspose.cells.drawing/texteffectformat/preset_shape) | Hämtar och ställer in den förinställda formtypen.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [set_text_effect(effect)](/cells/sv/python-net/aspose.cells.drawing/texteffectformat/set_text_effect/#MsoPresetTextEffect) | Ställer in den förinställda texteffekten.|



###  Exempel

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

###  Se även
* modul [aspose.cells.drawing](..)
