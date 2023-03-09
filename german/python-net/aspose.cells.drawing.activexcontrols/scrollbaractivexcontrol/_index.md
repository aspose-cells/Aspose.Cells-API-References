---
title: ScrollBarActiveXControl Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 100
url: /de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/
is_root: false
---
##  ScrollBarActiveXControl Klasse
Stellt das ScrollBar-Steuerelement dar.



**Nachlass:** [ScrollBarActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol) → 
[SpinButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/de/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



Der Typ ScrollBarActiveXControl macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [workbook](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/workbook) | Ruft das [ActiveXControlBase.workbook](/cells/de/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook)-Objekt ab.|
| [type](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/type) | Ruft den Typ des ActiveX-Steuerelements ab.|
| [width](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/width) |Ruft die Breite des Steuerelements in Punkteinheiten ab und legt diese fest.|
| [height](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/height) | Ruft die Höhe des Steuerelements in Punkteinheiten ab und legt diese fest.|
| [mouse_icon](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/mouse_icon) | Ruft ein benutzerdefiniertes Symbol ab und legt es fest, das als Mauszeiger für das Steuerelement angezeigt wird.|
| [mouse_pointer](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/mouse_pointer) | Ruft den Symboltyp ab, der als Mauszeiger für das Steuerelement angezeigt wird, und legt diesen fest.|
| [fore_ole_color](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/fore_ole_color) | Ruft die alte Farbe des Vordergrunds ab und legt sie fest.|
| [back_ole_color](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/back_ole_color) | Ruft die Ole-Farbe des Hintergrunds ab und legt sie fest.|
| [is_visible](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_visible) | Gibt an, ob dieses Steuerelement sichtbar ist.|
| [shadow](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/shadow) | Gibt an, ob ein Schatten angezeigt werden soll.|
| [linked_cell](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/linked_cell) | Ruft die verknüpfte Zelle ab und legt sie fest.|
| [list_fill_range](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/list_fill_range) | Ruft den Füllbereich der Liste ab und legt ihn fest.|
| [data](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/data) | Ruft die Binärdaten des Steuerelements ab und legt sie fest.|
| [is_enabled](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_enabled) | Gibt an, ob das Steuerelement den Fokus erhalten und auf vom Benutzer generierte Ereignisse reagieren kann.|
| [is_locked](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_locked) | Gibt an, ob Daten im Steuerelement zur Bearbeitung gesperrt sind.|
| [is_transparent](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_transparent) | Gibt an, ob das Steuerelement transparent ist.|
| [is_auto_size](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_auto_size) | Gibt an, ob die Größe des Steuerelements automatisch geändert wird, um seinen gesamten Inhalt anzuzeigen.|
| [ime_mode](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/ime_mode) |Ruft den standardmäßigen Laufzeitmodus des Eingabemethoden-Editors für das Steuerelement ab und legt diesen fest, wenn es den Fokus erhält.|
| [font](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/font) | Stellt die Schriftart des Steuerelements dar.|
| [text_align](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/text_align) | Stellt dar, wie der vom Steuerelement verwendete Text ausgerichtet wird.|
| [min](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/min) | Ruft den akzeptablen Mindestwert ab und legt ihn fest.|
| [max](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/max) | Ruft den maximal akzeptablen Wert ab und legt ihn fest.|
| [position](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/position) | Ruft den Wert ab und legt ihn fest.|
| [small_change](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/small_change) | Ruft den Betrag ab, um den sich die Position-Eigenschaft ändert, und legt diesen fest|
| [orientation](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/orientation) | Ruft ab und legt fest, ob SpinButton oder ScrollBar vertikal oder horizontal ausgerichtet ist.|
| [large_change](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/large_change) | Ruft den Betrag ab, um den sich die Position-Eigenschaft ändert, und legt diesen fest|



###  Beispiele

```python
from aspose import pycore
from aspose.cells import Workbook
from aspose.cells.drawing.activexcontrols import ControlType, ScrollBarActiveXControl

# Initialize a new workbook.
book = Workbook()
# Add a ToggleButtonActiveXControl.
shape = book.worksheets[0].shapes.add_active_x_control(ControlType.SCROLL_BAR, 1, 0, 1, 0, 100, 50)
activeXControl = pycore.cast(ScrollBarActiveXControl, shape.active_x_control)
# do your business
# Save the excel file.
book.save("exmaple.xlsx")

```

###  Siehe auch
* Modul [aspose.cells.drawing.activexcontrols](..)
* Klasse [ActiveXControl](/cells/de/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* Klasse [ActiveXControlBase](/cells/de/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* Klasse [ScrollBarActiveXControl](/cells/de/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol)
* Klasse [SpinButtonActiveXControl](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol)
