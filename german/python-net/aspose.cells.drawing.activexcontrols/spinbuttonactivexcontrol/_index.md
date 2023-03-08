---
title: SpinButtonActiveXControl Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 110
url: /de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/
is_root: false
---
##  SpinButtonActiveXControl Klasse
Stellt das SpinButton-Steuerelement dar.



**Nachlass:** [SpinButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/de/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



Der Typ SpinButtonActiveXControl macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [workbook](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/workbook) | Ruft das [ActiveXControlBase.workbook](/cells/de/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook)-Objekt ab.|
| [type](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type) | Ruft den Typ des ActiveX-Steuerelements ab.|
| [width](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/width) | Ruft die Breite des Steuerelements in Punkteinheiten ab und legt sie fest.|
| [height](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/height) | Ruft die Höhe des Steuerelements in Punkteinheiten ab und legt sie fest.|
| [mouse_icon](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/mouse_icon) | Ruft ein benutzerdefiniertes Symbol ab und legt es fest, das als Mauszeiger für das Steuerelement angezeigt wird.|
| [mouse_pointer](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/mouse_pointer) |Ruft den Symboltyp ab, der als Mauszeiger für das Steuerelement angezeigt wird, und legt diesen fest.|
| [fore_ole_color](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/fore_ole_color) | Ruft die alte Farbe des Vordergrunds ab und legt sie fest.|
| [back_ole_color](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/back_ole_color) | Ruft die Ole-Farbe des Hintergrunds ab und legt sie fest.|
| [is_visible](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_visible) | Gibt an, ob dieses Steuerelement sichtbar ist.|
| [shadow](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/shadow) | Gibt an, ob ein Schatten angezeigt werden soll.|
| [linked_cell](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/linked_cell) | Ruft die verknüpfte Zelle ab und legt sie fest.|
| [list_fill_range](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/list_fill_range) | Ruft den Füllbereich der Liste ab und legt ihn fest.|
| [data](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/data) | Ruft die Binärdaten des Steuerelements ab und legt sie fest.|
| [is_enabled](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_enabled) | Gibt an, ob das Steuerelement den Fokus erhalten und auf vom Benutzer generierte Ereignisse reagieren kann.|
| [is_locked](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_locked) | Gibt an, ob Daten im Steuerelement zur Bearbeitung gesperrt sind.|
| [is_transparent](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_transparent) |Gibt an, ob das Steuerelement transparent ist.|
| [is_auto_size](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_auto_size) | Gibt an, ob die Größe des Steuerelements automatisch geändert wird, um seinen gesamten Inhalt anzuzeigen.|
| [ime_mode](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/ime_mode) | Ruft den standardmäßigen Laufzeitmodus des Eingabemethoden-Editors für das Steuerelement ab und legt diesen fest, wenn es den Fokus erhält.|
| [font](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/font) | Stellt die Schriftart des Steuerelements dar.|
| [text_align](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/text_align) | Stellt dar, wie der vom Steuerelement verwendete Text ausgerichtet wird.|
| [min](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min) | Ruft den akzeptablen Mindestwert ab und legt ihn fest.|
| [max](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max) |Ruft den maximal akzeptablen Wert ab und legt ihn fest.|
| [position](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position) | Ruft den Wert ab und legt ihn fest.|
| [small_change](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/small_change) | Ruft den Betrag ab, um den sich die Position-Eigenschaft ändert, und legt diesen fest|
| [orientation](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation) | Ruft ab und legt fest, ob SpinButton oder ScrollBar vertikal oder horizontal ausgerichtet ist.|



###  Beispiel

```python
from aspose import pycore
from aspose.cells import Workbook
from aspose.cells.drawing.activexcontrols import ControlType, SpinButtonActiveXControl

# Initialize a new workbook.
book = Workbook()
# Add a ToggleButtonActiveXControl.
shape = book.worksheets[0].shapes.add_active_x_control(ControlType.SPIN_BUTTON, 1, 0, 1, 0, 100, 50)
activeXControl = pycore.cast(SpinButtonActiveXControl, shape.active_x_control)
# do your business
# Save the excel file.
book.save("exmaple.xlsx")

```

###  Siehe auch
* Modul [aspose.cells.drawing.activexcontrols](..)
* Klasse [ActiveXControl](/cells/de/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* Klasse [ActiveXControlBase](/cells/de/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* Klasse [SpinButtonActiveXControl](/cells/de/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol)
