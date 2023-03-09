---
title: ToggleButtonActiveXControl klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 130
url: /sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/
is_root: false
---
##  ToggleButtonActiveXControl klass
Representerar en ToggleButton ActiveX-kontroll.



**Arv:** [ToggleButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



Typen ToggleButtonActiveXControl avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [workbook](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/workbook) | Hämtar objektet [ActiveXControlBase.workbook](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook).|
| [type](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/type) | Hämtar typen av ActiveX-kontroll.|
| [width](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/width) | Hämtar och ställer in kontrollens bredd i poängenhet.|
| [height](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/height) | Får och ställer in höjden på kontrollen i poängenhet.|
| [mouse_icon](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_icon) | Hämtar och ställer in en anpassad ikon som ska visas som muspekare för kontrollen.|
| [mouse_pointer](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_pointer) |Hämtar och ställer in typen av ikon som visas som muspekare för kontrollen.|
| [fore_ole_color](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/fore_ole_color) | Får och ställer in olefärgen på förgrunden.|
| [back_ole_color](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/back_ole_color) | Hämtar och ställer in ole-färgen på bakgrunden.|
| [is_visible](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_visible) | Indikerar om denna kontroll är synlig.|
| [shadow](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/shadow) | Indikerar om en skugga ska visas.|
| [linked_cell](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/linked_cell) | Hämtar och ställer in den länkade cellen.|
| [list_fill_range](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/list_fill_range) | Hämtar och ställer in listfyllningsintervallet.|
| [data](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/data) | Hämtar och ställer in kontrollens binära data.|
| [is_enabled](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_enabled) | Indikerar om kontrollen kan ta emot fokus och svara på användargenererade händelser.|
| [is_locked](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_locked) | Indikerar om data i kontrollen är låst för redigering.|
| [is_transparent](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_transparent) |Indikerar om kontrollen är transparent.|
| [is_auto_size](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_auto_size) | Indikerar om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet.|
| [ime_mode](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/ime_mode) | Hämtar och ställer in standardkörtidsläget för Input Method Editor för kontrollen när den tar emot fokus.|
| [font](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/font) | Representerar kontrollens teckensnitt.|
| [text_align](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/text_align) | Representerar hur man justerar texten som används av kontrollen.|
| [caption](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/caption) | Hämtar och ställer in den beskrivande texten som visas på en kontroll.|
| [picture_position](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture_position) | Hämtar och ställer in platsen för kontrollens bild i förhållande till dess bildtext.|
| [special_effect](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/special_effect) | Får och ställer in kontrollens specialeffekt.|
| [picture](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture) |Hämtar och ställer in bildens data.|
| [accelerator](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/accelerator) | Hämtar och ställer in gasknappen för kontrollen.|
| [value](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/value) | Indikerar om kontrollen är kontrollerad eller inte.|
| [is_triple_state](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_triple_state) | Indikerar hur den angivna kontrollen kommer att visa nollvärden.|



###  Exempel

```python
from aspose import pycore
from aspose.cells import Workbook
from aspose.cells.drawing.activexcontrols import ControlType, ToggleButtonActiveXControl

# Initialize a new workbook.
book = Workbook()
# Add a ToggleButtonActiveXControl.
shape = book.worksheets[0].shapes.add_active_x_control(ControlType.TOGGLE_BUTTON, 1, 0, 1, 0, 100, 50)
activeXControl = pycore.cast(ToggleButtonActiveXControl, shape.active_x_control)
# do your business
# Save the excel file.
book.save("exmaple.xlsx")

```

###  Se även
* modul [aspose.cells.drawing.activexcontrols](..)
* klass [ActiveXControl](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* klass [ActiveXControlBase](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* klass [ToggleButtonActiveXControl](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol)
