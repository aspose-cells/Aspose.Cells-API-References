---
title: ToggleButtonActiveXControl clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 130
url: /es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/
is_root: false
---
##  ToggleButtonActiveXControl clase
Representa un control ActiveX ToggleButton.



**Herencia:** [ToggleButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/es/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



El tipo ToggleButtonActiveXControl expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [workbook](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/workbook) | Obtiene el objeto [ActiveXControlBase.workbook](/cells/es/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook).|
| [type](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/type) | Obtiene el tipo del control ActiveX.|
| [width](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/width) |Obtiene y establece el ancho del control en unidades de puntos.|
| [height](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/height) | Obtiene y establece el alto del control en unidades de puntos.|
| [mouse_icon](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_icon) | Obtiene y establece un icono personalizado para mostrar como el puntero del mouse para el control.|
| [mouse_pointer](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_pointer) | Obtiene y establece el tipo de icono que se muestra como el puntero del mouse para el control.|
| [fore_ole_color](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/fore_ole_color) | Obtiene y establece el color antiguo del primer plano.|
| [back_ole_color](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/back_ole_color) | Obtiene y establece el color antiguo del fondo.|
| [is_visible](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_visible) | Indica si este control es visible.|
| [shadow](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/shadow) | Indica si mostrar una sombra.|
| [linked_cell](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/linked_cell) | Obtiene y establece la celda vinculada.|
| [list_fill_range](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/list_fill_range) | Obtiene y establece el rango de relleno de la lista.|
| [data](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/data) | Obtiene y establece los datos binarios del control.|
| [is_enabled](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_enabled) | Indica si el control puede recibir el foco y responder a los eventos generados por el usuario.|
| [is_locked](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_locked) | Indica si los datos del control están bloqueados para su edición.|
| [is_transparent](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_transparent) | Indica si el control es transparente.|
| [is_auto_size](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_auto_size) | Indica si el control cambiará de tamaño automáticamente para mostrar todo su contenido.|
| [ime_mode](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/ime_mode) |Obtiene y establece el modo de tiempo de ejecución predeterminado del Editor de métodos de entrada para el control cuando recibe el foco.|
| [font](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/font) | Representa la fuente del control.|
| [text_align](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/text_align) | Representa cómo alinear el texto utilizado por el control.|
| [caption](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/caption) | Obtiene y establece el texto descriptivo que aparece en un control.|
| [picture_position](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture_position) | Obtiene y establece la ubicación de la imagen del control en relación con su título.|
| [special_effect](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/special_effect) | Obtiene y establece el efecto especial del control.|
| [picture](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture) | Obtiene y establece los datos de la imagen.|
| [accelerator](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/accelerator) | Obtiene y establece la tecla aceleradora del control.|
| [value](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/value) |Indica si el control está marcado o no.|
| [is_triple_state](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_triple_state) | Indica cómo el control especificado mostrará valores nulos.|



###  Ejemplos

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

###  Ver también
* módulo [aspose.cells.drawing.activexcontrols](..)
* clase [ActiveXControl](/cells/es/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* clase [ActiveXControlBase](/cells/es/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* clase [ToggleButtonActiveXControl](/cells/es/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol)
