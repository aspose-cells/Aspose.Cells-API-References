---
title: Range clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1250
url: /es/python-net/aspose.cells/range/
is_root: false
---
##  Range clase
Encapsula el objeto que representa un rango de celdas dentro de una hoja de cálculo.



El tipo Range expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [current_region](/cells/es/python-net/aspose.cells/range/current_region) |Devuelve un objeto Range que representa la región actual.<br/> La región actual es un rango limitado por cualquier combinación de filas y columnas en blanco.|
| [hyperlinks](/cells/es/python-net/aspose.cells/range/hyperlinks) | Obtiene todos los hipervínculos del intervalo.|
| [row_count](/cells/es/python-net/aspose.cells/range/row_count) | Obtiene el recuento de filas en el rango.|
| [column_count](/cells/es/python-net/aspose.cells/range/column_count) | Obtiene el recuento de columnas en el rango.|
| [cell_count](/cells/es/python-net/aspose.cells/range/cell_count) | Obtiene todos los recuentos de celdas en el rango.|
| [name](/cells/es/python-net/aspose.cells/range/name) | Obtiene o establece el nombre del rango.|
| [refers_to](/cells/es/python-net/aspose.cells/range/refers_to) | Obtiene el rango al que se refiere.|
| [address](/cells/es/python-net/aspose.cells/range/address) | Obtiene la dirección del rango.|
| [left](/cells/es/python-net/aspose.cells/range/left) | Obtiene la distancia, en puntos, desde el borde izquierdo de la columna A hasta el borde izquierdo del rango.|
| [top](/cells/es/python-net/aspose.cells/range/top) | Obtiene la distancia, en puntos, desde el borde superior de la fila 1 hasta el borde superior del rango.|
| [width](/cells/es/python-net/aspose.cells/range/width) | Obtiene el ancho de un rango en puntos.|
| [height](/cells/es/python-net/aspose.cells/range/height) | Obtiene el ancho de un rango en puntos.|
| [first_row](/cells/es/python-net/aspose.cells/range/first_row) | Obtiene el índice de la primera fila del rango.|
| [first_column](/cells/es/python-net/aspose.cells/range/first_column) | Obtiene el índice de la primera columna del rango.|
| [value](/cells/es/python-net/aspose.cells/range/value) | Obtiene y establece el valor del rango.|
| [column_width](/cells/es/python-net/aspose.cells/range/column_width) | Establece u obtiene el ancho de columna de este rango|
| [row_height](/cells/es/python-net/aspose.cells/range/row_height) | Establece u obtiene la altura de las filas en este rango|
| [entire_column](/cells/es/python-net/aspose.cells/range/entire_column) |Obtiene un objeto Range que representa la columna (o columnas) completa que contiene el rango especificado.|
| [entire_row](/cells/es/python-net/aspose.cells/range/entire_row) | Obtiene un objeto Range que representa toda la fila (o filas) que contiene el rango especificado.|
| [worksheet](/cells/es/python-net/aspose.cells/range/worksheet) | Obtiene el objeto [Range.worksheet](/cells/es/python-net/aspose.cells/range#worksheet) que contiene este rango.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [auto_fill(target)](/cells/es/python-net/aspose.cells/range/auto_fill/#Range) | Automático todo llena el rango objetivo.|
| [auto_fill(target, auto_fill_type)](/cells/es/python-net/aspose.cells/range/auto_fill/#Range-AutoFillType) | Automático todo llena el rango objetivo.|
| [set_style(style, explicit_flag)](/cells/es/python-net/aspose.cells/range/set_style/#Style-bool) | Aplicar el estilo de celda.|
| [set_style(style)](/cells/es/python-net/aspose.cells/range/set_style/#Style) | Establece el estilo del rango.|
| [set_outline_borders(border_style, border_color)](/cells/es/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-CellsColor) | Establece los bordes del contorno alrededor de un rango de celdas con el mismo estilo y color de borde.|
| [set_outline_borders(border_style, border_color)](/cells/es/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-aspose.pydrawing.Color) | Establece los bordes del contorno alrededor de un rango de celdas con el mismo estilo y color de borde.|
| [set_outline_borders(border_styles, border_colors)](/cells/es/python-net/aspose.cells/range/set_outline_borders/#list-aspose.pydrawing.Color[]) | Establece bordes de línea alrededor de un rango de celdas.|
| [set_outline_border(border_edge, border_style, border_color)](/cells/es/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-CellsColor) | Establece el borde del contorno alrededor de un rango de celdas.|
| [set_outline_border(border_edge, border_style, border_color)](/cells/es/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-aspose.pydrawing.Color) | Establece el borde del contorno alrededor de un rango de celdas.|
| [copy(range, options)](/cells/es/python-net/aspose.cells/range/copy/#Range-PasteOptions) | Copiando el rango con opciones especiales de pegado.|
| [copy(range)](/cells/es/python-net/aspose.cells/range/copy/#Range) | Copia datos (incluidas fórmulas), formato, objetos de dibujo, etc. de un rango de origen.|
| [get_enumerator()](/cells/es/python-net/aspose.cells/range/get_enumerator/#) | Obtiene el enumerador de las celdas de este rango.|
| [is_intersect(range)](/cells/es/python-net/aspose.cells/range/is_intersect/#Range) | Indica si el rango es de intersección.|
| [intersect(range)](/cells/es/python-net/aspose.cells/range/intersect/#Range) | Devuelve un objeto [Range](/cells/es/python-net/aspose.cells/range) que representa la intersección rectangular de dos rangos.|
| [union(range)](/cells/es/python-net/aspose.cells/range/union/#Range) | Devuelve la unión de dos rangos.|
| [merge()](/cells/es/python-net/aspose.cells/range/merge/#) | Combina un rango de celdas en una sola celda.|
| [un_merge()](/cells/es/python-net/aspose.cells/range/un_merge/#) |Separa las celdas combinadas de este rango.|
| [put_value(string_value, is_converted, set_style)](/cells/es/python-net/aspose.cells/range/put_value/#str-bool-bool) | Pone un valor en el rango, si corresponde, el valor se convertirá a otro tipo de datos y el formato de número de celda se restablecerá.|
| [apply_style(style, flag)](/cells/es/python-net/aspose.cells/range/apply_style/#Style-StyleFlag) | Aplica formatos para toda una gama.|
| [set_inside_borders(border_edge, line_style, border_color)](/cells/es/python-net/aspose.cells/range/set_inside_borders/#BorderType-CellBorderType-CellsColor) | Establecer dentro de los límites del rango.|
| [move_to(dest_row, dest_column)](/cells/es/python-net/aspose.cells/range/move_to/#int-int) | Mueve el rango actual al rango de destino.|
| [copy_data(range)](/cells/es/python-net/aspose.cells/range/copy_data/#Range) | Copia datos de celda (incluidas fórmulas) de un rango de origen.|
| [copy_value(range)](/cells/es/python-net/aspose.cells/range/copy_value/#Range) | Copia el valor de la celda de un rango de origen.|
| [copy_style(range)](/cells/es/python-net/aspose.cells/range/copy_style/#Range) | Copia la configuración de estilo de un rango de origen.|
| [get_cell_or_null(row_offset, column_offset)](/cells/es/python-net/aspose.cells/range/get_cell_or_null/#int-int) | Obtiene el objeto [Cell](/cells/es/python-net/aspose.cells/cell) o nulo en este rango.|
| [get_offset(row_offset, column_offset)](/cells/es/python-net/aspose.cells/range/get_offset/#int-int) | Obtiene el rango [Range](/cells/es/python-net/aspose.cells/range) por desplazamiento.|



###  Ejemplos

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
#  Create a range (A1:D3).
range = cells.create_range("A1", "D3")
#  Set value to the range.
range.value = "Hello"
# Save the Excel file
workbook.save("book1.xlsm")

```

###  Ver también
* módulo [aspose.cells](..)
* clase [Cell](/cells/es/python-net/aspose.cells/cell)
* clase [Range](/cells/es/python-net/aspose.cells/range)
