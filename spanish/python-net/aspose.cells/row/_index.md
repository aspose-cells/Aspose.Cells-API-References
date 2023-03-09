---
title: Row clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1300
url: /es/python-net/aspose.cells/row/
is_root: false
---
##  Row clase
Representa una sola fila en una hoja de cálculo.



El tipo Row expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [is_blank](/cells/es/python-net/aspose.cells/row/is_blank) | Indica si la fila contiene algún dato.|
| [is_collapsed](/cells/es/python-net/aspose.cells/row/is_collapsed) | si la fila está colapsada|
| [height](/cells/es/python-net/aspose.cells/row/height) | Obtiene y establece el alto de la fila en unidades de Puntos.|
| [is_hidden](/cells/es/python-net/aspose.cells/row/is_hidden) | Indica si la fila está oculta.|
| [index](/cells/es/python-net/aspose.cells/row/index) | Obtiene el índice de esta fila.|
| [group_level](/cells/es/python-net/aspose.cells/row/group_level) | Obtiene el nivel de grupo de la fila.|
| [is_height_matched](/cells/es/python-net/aspose.cells/row/is_height_matched) | Indica que la altura de fila y la altura de fuente predeterminada coinciden.|
| [style](/cells/es/python-net/aspose.cells/row/style) | Representa el estilo de esta fila.|
| [has_custom_style](/cells/es/python-net/aspose.cells/row/has_custom_style) | Indica si esta fila tiene una configuración de estilo personalizada (diferente a la predeterminada heredada del libro de trabajo).|
| [first_cell](/cells/es/python-net/aspose.cells/row/first_cell) | Obtiene el primer objeto de celda de la fila.|
| [first_data_cell](/cells/es/python-net/aspose.cells/row/first_data_cell) | Obtiene la primera celda que no está en blanco de la fila.|
| [last_cell](/cells/es/python-net/aspose.cells/row/last_cell) |Obtiene el último objeto de celda de la fila.|
| [last_data_cell](/cells/es/python-net/aspose.cells/row/last_data_cell) | Obtiene la última celda que no está en blanco de la fila.|



Obtiene el celular.
###  indexador
| Nombre| Descripción|
| :- | :- |
| [index] | El índice de la columna|


###  Métodos
| Método| Descripción|
| :- | :- |
| [get_cell_by_index(index)](/cells/es/python-net/aspose.cells/row/get_cell_by_index/#int) | Obtenga la celda por índice específico en la lista.|
| [get_cell_or_null(column)](/cells/es/python-net/aspose.cells/row/get_cell_or_null/#int) | Obtiene la celda o nulo en el índice específico.|
| [get_style()](/cells/es/python-net/aspose.cells/row/get_style/#) | Obtiene el estilo de esta fila.|
| [set_style(style)](/cells/es/python-net/aspose.cells/row/set_style/#Style) | Establece el estilo de esta fila.|
| [copy_settings(source, check_style)](/cells/es/python-net/aspose.cells/row/copy_settings/#Row-bool) | Copie la configuración de la fila, como estilo, altura, visibilidad, etc.|
| [apply_style(style, flag)](/cells/es/python-net/aspose.cells/row/apply_style/#Style-StyleFlag) | Aplica formatos para una fila completa.|
| [equals(row)](/cells/es/python-net/aspose.cells/row/equals/#Row) | Comprueba si este objeto hace referencia a la misma fila con otro objeto de fila.|



###  Ejemplo

```python
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
style = workbook.create_style()
# Setting the background color to Blue
style.background_color = Color.blue
# Setting the foreground color to Red
style.foreground_color = Color.red
# setting Background Pattern
style.pattern = BackgroundType.DIAGONAL_STRIPE
# New Style Flag
styleFlag = StyleFlag()
# Set All Styles
styleFlag.all = True
# Get first row
row = worksheet.cells.rows[0]
# Apply Style to first row
row.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Ver también
* módulo [aspose.cells](..)
