---
title: ListObject clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells.tables/listobject/
is_root: false
---
##  ListObject clase
Representa un objeto de lista en una hoja de cálculo.
 El objeto ListObject es miembro de la colección ListObjects.
La colección ListObjects contiene todos los objetos de lista en una hoja de trabajo.



El tipo ListObject expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [start_row](/cells/es/python-net/aspose.cells.tables/listobject/start_row) | Obtiene la fila inicial del rango.|
| [start_column](/cells/es/python-net/aspose.cells.tables/listobject/start_column) | Obtiene la columna inicial del rango.|
| [end_row](/cells/es/python-net/aspose.cells.tables/listobject/end_row) | Obtiene la última fila del rango.|
| [end_column](/cells/es/python-net/aspose.cells.tables/listobject/end_column) |Obtiene la última columna del rango.|
| [list_columns](/cells/es/python-net/aspose.cells.tables/listobject/list_columns) | Obtiene ListColumns de ListObject.|
| [show_header_row](/cells/es/python-net/aspose.cells.tables/listobject/show_header_row) | Obtiene y establece si ListObject muestra la fila de encabezado.|
| [show_totals](/cells/es/python-net/aspose.cells.tables/listobject/show_totals) | Obtiene y establece si este ListObject muestra la fila total.|
| [data_range](/cells/es/python-net/aspose.cells.tables/listobject/data_range) | Obtiene el rango de datos de ListObject.|
| [query_table](/cells/es/python-net/aspose.cells.tables/listobject/query_table) | Obtiene la QueryTable vinculada.|
| [data_source_type](/cells/es/python-net/aspose.cells.tables/listobject/data_source_type) | Obtiene el tipo de origen de datos de la tabla.|
| [auto_filter](/cells/es/python-net/aspose.cells.tables/listobject/auto_filter) | Obtiene filtro automático.|
| [display_name](/cells/es/python-net/aspose.cells.tables/listobject/display_name) | Obtiene y establece el nombre para mostrar.|
| [comment](/cells/es/python-net/aspose.cells.tables/listobject/comment) | Obtiene y establece el comentario de la tabla.|
| [show_table_style_first_column](/cells/es/python-net/aspose.cells.tables/listobject/show_table_style_first_column) | Indica si la primera columna de la tabla debe tener el estilo aplicado.|
| [show_table_style_last_column](/cells/es/python-net/aspose.cells.tables/listobject/show_table_style_last_column) | Indica si la última columna de la tabla debe tener el estilo aplicado.|
| [show_table_style_row_stripes](/cells/es/python-net/aspose.cells.tables/listobject/show_table_style_row_stripes) | Indica si se aplica el formato de franja de fila.|
| [show_table_style_column_stripes](/cells/es/python-net/aspose.cells.tables/listobject/show_table_style_column_stripes) | Indica si se aplica el formato de franja de columna.|
| [table_style_type](/cells/es/python-net/aspose.cells.tables/listobject/table_style_type) | Obtiene y el estilo de tabla integrado.|
| [table_style_name](/cells/es/python-net/aspose.cells.tables/listobject/table_style_name) | Obtiene y establece el nombre del estilo de la tabla.|
| [xml_map](/cells/es/python-net/aspose.cells.tables/listobject/xml_map) | Obtiene un [ListObject.xml_map](/cells/es/python-net/aspose.cells.tables/listobject#xml_map) utilizado para esta lista.|
| [alternative_text](/cells/es/python-net/aspose.cells.tables/listobject/alternative_text) | Obtiene y establece el texto alternativo.|
| [alternative_description](/cells/es/python-net/aspose.cells.tables/listobject/alternative_description) | Obtiene y establece la descripción alternativa.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [convert_to_range()](/cells/es/python-net/aspose.cells.tables/listobject/convert_to_range/#) | Convierte la tabla a rango.|
| [convert_to_range(options)](/cells/es/python-net/aspose.cells.tables/listobject/convert_to_range/#TableToRangeOptions) | Convierte la tabla a rango.|
| [resize(start_row, start_column, end_row, end_column, has_headers)](/cells/es/python-net/aspose.cells.tables/listobject/resize/#int-int-int-int-bool) | Cambiar el tamaño del rango del objeto de la lista.|
| [put_cell_value(row_offset, column_offset, value)](/cells/es/python-net/aspose.cells.tables/listobject/put_cell_value/#int-int-any) | Poner el valor a la celda.|
| [update_column_name()](/cells/es/python-net/aspose.cells.tables/listobject/update_column_name/#) |Actualiza el nombre de todas las columnas de la lista de la hoja de trabajo.|
| [filter()](/cells/es/python-net/aspose.cells.tables/listobject/filter/#) | Filtrar la tabla.|
| [apply_style_to_range()](/cells/es/python-net/aspose.cells.tables/listobject/apply_style_to_range/#) | Aplique el estilo de tabla al rango.|



###  Ejemplo

```python
from aspose.cells import CellsHelper, Workbook
from aspose.cells.tables import TotalsCalculation

workbook = Workbook()
cells = workbook.worksheets[0].cells
for i in range(5):
    cells.get(0, i).put_value(CellsHelper.column_index_to_name(i))
for row in range(1, 10):
    for column in range(5):
        cells.get(row, column).put_value(row * column)
tables = workbook.worksheets[0].list_objects
index = tables.add(0, 0, 9, 4, True)
table = tables[0]
table.show_totals = True
table.list_columns[4].totals_calculation = TotalsCalculation.SUM
workbook.save(r"Book1.xlsx")

```

###  Ver también
* módulo [aspose.cells.tables](..)
