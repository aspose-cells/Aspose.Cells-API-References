---
title: Column clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 260
url: /es/python-net/aspose.cells/column/
is_root: false
---
##  Column clase
Representa una sola columna en una hoja de cálculo.



El tipo Column expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [index](/cells/es/python-net/aspose.cells/column/index) | Obtiene el índice de esta columna.|
| [width](/cells/es/python-net/aspose.cells/column/width) | Obtiene y establece el ancho de columna en unidades de caracteres.|
| [group_level](/cells/es/python-net/aspose.cells/column/group_level) |Obtiene el nivel de grupo de la columna.|
| [is_hidden](/cells/es/python-net/aspose.cells/column/is_hidden) | Indica si la columna está oculta.|
| [has_custom_style](/cells/es/python-net/aspose.cells/column/has_custom_style) | Indica si esta columna tiene una configuración de estilo personalizada (diferente a la predeterminada heredada del libro de trabajo).|
| [style](/cells/es/python-net/aspose.cells/column/style) | Obtiene el estilo de esta columna.|
| [is_collapsed](/cells/es/python-net/aspose.cells/column/is_collapsed) | si la columna está colapsada|


###  Métodos
| Método| Descripción|
| :- | :- |
| [apply_style(style, flag)](/cells/es/python-net/aspose.cells/column/apply_style/#Style-StyleFlag) | Aplica formatos para una columna completa.|
| [get_style()](/cells/es/python-net/aspose.cells/column/get_style/#) | Obtiene el estilo de esta columna.|
| [set_style(style)](/cells/es/python-net/aspose.cells/column/set_style/#Style) | Establece el estilo de esta columna.|



###  Ejemplos

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
# Get first Column
column = worksheet.cells.columns[0]
# Apply Style to first Column
column.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Ver también
* módulo [aspose.cells](..)
