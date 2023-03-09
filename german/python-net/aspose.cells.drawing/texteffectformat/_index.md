---
title: TextEffectFormat Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 700
url: /de/python-net/aspose.cells.drawing/texteffectformat/
is_root: false
---
##  TextEffectFormat Klasse
Enthält Eigenschaften und Methoden, die für WordArt-Objekte gelten.



Der Typ TextEffectFormat macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [text](/cells/de/python-net/aspose.cells.drawing/texteffectformat/text) | Der Text in der WordArt.|
| [font_name](/cells/de/python-net/aspose.cells.drawing/texteffectformat/font_name) | Der Name der Schriftart, die in der WordArt verwendet wird.|
| [font_bold](/cells/de/python-net/aspose.cells.drawing/texteffectformat/font_bold) | Gibt an, ob die Schriftart fett ist.|
| [font_italic](/cells/de/python-net/aspose.cells.drawing/texteffectformat/font_italic) | Gibt an, ob die Schriftart kursiv ist.|
| [rotated_chars](/cells/de/python-net/aspose.cells.drawing/texteffectformat/rotated_chars) | Bei „true“ werden die Zeichen im angegebenen WordArt-Objekt um 90 Grad relativ zur Begrenzungsform des WordArt-Objekts gedreht.|
| [font_size](/cells/de/python-net/aspose.cells.drawing/texteffectformat/font_size) | Die Größe (in Punkten) der in der WordArt verwendeten Schriftart.|
| [preset_shape](/cells/de/python-net/aspose.cells.drawing/texteffectformat/preset_shape) | Ruft den voreingestellten Formtyp ab und legt ihn fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [set_text_effect(effect)](/cells/de/python-net/aspose.cells.drawing/texteffectformat/set_text_effect/#MsoPresetTextEffect) | Legt den voreingestellten Texteffekt fest.|



###  Beispiele

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

###  Siehe auch
* Modul [aspose.cells.drawing](..)
