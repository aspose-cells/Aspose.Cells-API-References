---
title: SpinButtonActiveXControl klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 110
url: /sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/
is_root: false
---
##  SpinButtonActiveXControl klass
Representerar SpinButton-kontrollen.



**Arv:** [SpinButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



Typen SpinButtonActiveXControl avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [workbook](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/workbook) | Hämtar objektet [ActiveXControlBase.workbook](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook).|
| [type](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type) | Hämtar typen av ActiveX-kontroll.|
| [width](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/width) |Hämtar och ställer in kontrollens bredd i poängenhet.|
| [height](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/height) | Får och ställer in höjden på kontrollen i poängenhet.|
| [mouse_icon](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/mouse_icon) | Hämtar och ställer in en anpassad ikon som ska visas som muspekare för kontrollen.|
| [mouse_pointer](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/mouse_pointer) | Hämtar och ställer in typen av ikon som visas som muspekare för kontrollen.|
| [fore_ole_color](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/fore_ole_color) | Får och ställer in olefärgen på förgrunden.|
| [back_ole_color](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/back_ole_color) | Hämtar och ställer in ole-färgen på bakgrunden.|
| [is_visible](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_visible) | Indikerar om denna kontroll är synlig.|
| [shadow](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/shadow) | Indikerar om en skugga ska visas.|
| [linked_cell](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/linked_cell) | Hämtar och ställer in den länkade cellen.|
| [list_fill_range](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/list_fill_range) | Hämtar och ställer in listfyllningsintervallet.|
| [data](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/data) | Hämtar och ställer in kontrollens binära data.|
| [is_enabled](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_enabled) | Indikerar om kontrollen kan ta emot fokus och svara på användargenererade händelser.|
| [is_locked](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_locked) | Indikerar om data i kontrollen är låst för redigering.|
| [is_transparent](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_transparent) | Indikerar om kontrollen är transparent.|
| [is_auto_size](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_auto_size) | Indikerar om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet.|
| [ime_mode](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/ime_mode) |Hämtar och ställer in standardkörtidsläget för Input Method Editor för kontrollen när den tar emot fokus.|
| [font](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/font) | Representerar kontrollens teckensnitt.|
| [text_align](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/text_align) | Representerar hur man justerar texten som används av kontrollen.|
| [min](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min) | Hämtar och ställer in det lägsta acceptabla värdet.|
| [max](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max) | Får och ställer in det högsta acceptabla värdet.|
| [position](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position) | Får och ställer in värdet.|
| [small_change](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/small_change) | Hämtar och ställer in det belopp med vilket positionsegenskapen ändras|
| [orientation](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation) | Hämtar och ställer in om SpinButton eller ScrollBar är orienterad vertikalt eller horisontellt.|



###  Exempel

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

###  Se även
* modul [aspose.cells.drawing.activexcontrols](..)
* klass [ActiveXControl](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* klass [ActiveXControlBase](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* klass [SpinButtonActiveXControl](/cells/sv/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol)
