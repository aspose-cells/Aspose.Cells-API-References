---
title: ScrollBarActiveXControl clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 100
url: /es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/
is_root: false
---
##  ScrollBarActiveXControl clase
Representa el control ScrollBar.



**Herencia:** [ScrollBarActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol) → 
[SpinButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/es/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



El tipo ScrollBarActiveXControl expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [workbook](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/workbook) | Obtiene el objeto [ActiveXControlBase.workbook](/cells/es/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook).|
| [type](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/type) | Obtiene el tipo del control ActiveX.|
| [width](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/width) | Obtiene y establece el ancho del control en unidades de puntos.|
| [height](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/height) | Obtiene y establece el alto del control en unidades de puntos.|
| [mouse_icon](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/mouse_icon) | Obtiene y establece un icono personalizado para mostrar como el puntero del mouse para el control.|
| [mouse_pointer](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/mouse_pointer) |Obtiene y establece el tipo de icono que se muestra como el puntero del mouse para el control.|
| [fore_ole_color](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/fore_ole_color) | Obtiene y establece el color antiguo del primer plano.|
| [back_ole_color](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/back_ole_color) | Obtiene y establece el color antiguo del fondo.|
| [is_visible](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_visible) | Indica si este control es visible.|
| [shadow](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/shadow) | Indica si mostrar una sombra.|
| [linked_cell](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/linked_cell) | Obtiene y establece la celda vinculada.|
| [list_fill_range](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/list_fill_range) | Obtiene y establece el rango de relleno de la lista.|
| [data](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/data) | Obtiene y establece los datos binarios del control.|
| [is_enabled](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_enabled) | Indica si el control puede recibir el foco y responder a los eventos generados por el usuario.|
| [is_locked](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_locked) | Indica si los datos del control están bloqueados para su edición.|
| [is_transparent](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_transparent) |Indica si el control es transparente.|
| [is_auto_size](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_auto_size) | Indica si el control cambiará de tamaño automáticamente para mostrar todo su contenido.|
| [ime_mode](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/ime_mode) | Obtiene y establece el modo de tiempo de ejecución predeterminado del Editor de métodos de entrada para el control cuando recibe el foco.|
| [font](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/font) | Representa la fuente del control.|
| [text_align](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/text_align) | Representa cómo alinear el texto utilizado por el control.|
| [min](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/min) | Obtiene y establece el valor mínimo aceptable.|
| [max](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/max) |Obtiene y establece el valor máximo aceptable.|
| [position](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/position) | Obtiene y establece el valor.|
| [small_change](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/small_change) | Obtiene y establece la cantidad por la que cambia la propiedad Position|
| [orientation](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/orientation) | Obtiene y establece si SpinButton o ScrollBar están orientados vertical u horizontalmente.|
| [large_change](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/large_change) | Obtiene y establece la cantidad por la que cambia la propiedad Position|



###  Ejemplo

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

###  Ver también
* módulo [aspose.cells.drawing.activexcontrols](..)
* clase [ActiveXControl](/cells/es/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* clase [ActiveXControlBase](/cells/es/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* clase [ScrollBarActiveXControl](/cells/es/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol)
* clase [SpinButtonActiveXControl](/cells/es/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol)
