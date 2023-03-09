---
title: AutoFilter clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 70
url: /es/python-net/aspose.cells/autofilter/
is_root: false
---
##  AutoFilter clase
Representa el filtrado automático para la hoja de cálculo especificada.



El tipo AutoFilter expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [sorter](/cells/es/python-net/aspose.cells/autofilter/sorter) | Obtiene el clasificador de datos.|
| [range](/cells/es/python-net/aspose.cells/autofilter/range) | Representa el rango al que se aplica el Autofiltro especificado.|
| [show_filter_button](/cells/es/python-net/aspose.cells/autofilter/show_filter_button) | Indica si el botón Autofiltro para esta columna está visible.|
| [filter_columns](/cells/es/python-net/aspose.cells/autofilter/filter_columns) | Obtiene la colección de las columnas de filtro.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [remove_filter(field_index, criteria)](/cells/es/python-net/aspose.cells/autofilter/remove_filter/#int-str) | Elimina un filtro para una columna de filtro.|
| [remove_filter(field_index)](/cells/es/python-net/aspose.cells/autofilter/remove_filter/#int) | Retire el filtro específico.|
| [custom(field_index, operator_type1, criteria1)](/cells/es/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any) | Filtra una lista con un criterio personalizado.|
| [custom(field_index, operator_type1, criteria1, is_and, operator_type2, criteria2)](/cells/es/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any-bool-FilterOperatorType-any) | Filtra una lista con criterios personalizados.|
| [refresh()](/cells/es/python-net/aspose.cells/autofilter/refresh/#) | Actualice los filtros automáticos para ocultar o mostrar las filas.|
| [refresh(hide_rows)](/cells/es/python-net/aspose.cells/autofilter/refresh/#bool) | Obtiene los índices de todas las filas ocultas.|
| [set_range(row, start_column, end_column)](/cells/es/python-net/aspose.cells/autofilter/set_range/#int-int-int) | Establece el rango al que se aplica el Autofiltro especificado.|
| [get_cell_area()](/cells/es/python-net/aspose.cells/autofilter/get_cell_area/#) | Obtiene el [CellArea](/cells/es/python-net/aspose.cells/cellarea) al que se aplica el Autofiltro especificado.|
| [add_filter(field_index, criteria)](/cells/es/python-net/aspose.cells/autofilter/add_filter/#int-str) | Agrega un filtro para una columna de filtro.|
| [add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/es/python-net/aspose.cells/autofilter/add_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Agrega un filtro de fecha.|
| [remove_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/es/python-net/aspose.cells/autofilter/remove_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Elimina un filtro de fecha.|
| [filter(field_index, criteria)](/cells/es/python-net/aspose.cells/autofilter/filter/#int-str) |Filtra una lista con criterios específicos.|
| [filter_top10(field_index, is_top, is_percent, item_count)](/cells/es/python-net/aspose.cells/autofilter/filter_top10/#int-bool-bool-int) | Filtrar los 10 elementos principales de la lista|
| [dynamic_filter(field_index, dynamic_filter_type)](/cells/es/python-net/aspose.cells/autofilter/dynamic_filter/#int-DynamicFilterType) | Añade un filtro dinámico.|
| [add_font_color_filter(field_index, color)](/cells/es/python-net/aspose.cells/autofilter/add_font_color_filter/#int-CellsColor) | Agrega un filtro de color de fuente.|
| [add_fill_color_filter(field_index, pattern, foreground_color, background_color)](/cells/es/python-net/aspose.cells/autofilter/add_fill_color_filter/#int-BackgroundType-CellsColor-CellsColor) | Agrega un filtro de color de relleno.|
| [add_icon_filter(field_index, icon_set_type, icon_id)](/cells/es/python-net/aspose.cells/autofilter/add_icon_filter/#int-IconSetType-int) | Añade un filtro de iconos.|
| [match_blanks(field_index)](/cells/es/python-net/aspose.cells/autofilter/match_blanks/#int) | Coincide con todas las celdas en blanco de la lista.|
| [match_non_blanks(field_index)](/cells/es/python-net/aspose.cells/autofilter/match_non_blanks/#int) | Haga coincidir todas las celdas que no están en blanco en la lista.|
| [show_all()](/cells/es/python-net/aspose.cells/autofilter/show_all/#) | Mostrar todas las filas.|



###  Ejemplo

```python
from aspose.cells import Workbook

# Creating a file stream containing the Excel file to be opened
# Instantiating a Workbook object
workbook = Workbook("template.xlsx")
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating AutoFilter by giving the cells range of the heading row
worksheet.auto_filter.range = "A1:B1"
# Filtering columns with specified values
worksheet.auto_filter.filter(1, "Bananas")
# Saving the modified Excel file.
workbook.save("output.xls")

```

###  Ver también
* módulo [aspose.cells](..)
* clase [CellArea](/cells/es/python-net/aspose.cells/cellarea)
