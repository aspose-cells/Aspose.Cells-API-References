---
title: PivotField clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 10
url: /es/python-net/aspose.cells.pivot/pivotfield/
is_root: false
---
##  PivotField clase
Representa un campo en un informe de tabla dinámica.



El tipo PivotField expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [pivot_items](/cells/es/python-net/aspose.cells.pivot/pivotfield/pivot_items) | Obtiene los elementos pivote del campo pivote|
| [range](/cells/es/python-net/aspose.cells.pivot/pivotfield/range) | Obtiene el rango de grupo del campo pivote|
| [is_calculated_field](/cells/es/python-net/aspose.cells.pivot/pivotfield/is_calculated_field) | Indica si el campo de tabla dinámica especificado es un campo calculado.|
| [base_index](/cells/es/python-net/aspose.cells.pivot/pivotfield/base_index) | Representa el índice de PivotField en los PivotFields base.|
| [position](/cells/es/python-net/aspose.cells.pivot/pivotfield/position) | Representa el índice de PivotField en PivotFields.|
| [name](/cells/es/python-net/aspose.cells.pivot/pivotfield/name) | Representa el nombre de PivotField.|
| [display_name](/cells/es/python-net/aspose.cells.pivot/pivotfield/display_name) | Representa el nombre para mostrar de PivotField.|
| [is_auto_subtotals](/cells/es/python-net/aspose.cells.pivot/pivotfield/is_auto_subtotals) | Indica si el campo especificado muestra subtotales automáticos. El valor predeterminado es verdadero.|
| [drag_to_column](/cells/es/python-net/aspose.cells.pivot/pivotfield/drag_to_column) | Indica si el campo especificado se puede arrastrar a la posición de la columna.<br/> El valor por defecto es verdadero.|
| [drag_to_hide](/cells/es/python-net/aspose.cells.pivot/pivotfield/drag_to_hide) | Indica si el campo especificado se puede arrastrar a la posición oculta.<br/> El valor por defecto es verdadero.|
| [drag_to_row](/cells/es/python-net/aspose.cells.pivot/pivotfield/drag_to_row) | Indica si el campo especificado se puede arrastrar a la posición de la fila.<br/> El valor por defecto es verdadero.|
| [drag_to_page](/cells/es/python-net/aspose.cells.pivot/pivotfield/drag_to_page) | Indica si el campo especificado se puede arrastrar a la posición de la página.<br/> El valor por defecto es verdadero.|
| [drag_to_data](/cells/es/python-net/aspose.cells.pivot/pivotfield/drag_to_data) |Indica si el campo especificado se puede arrastrar a la posición de los datos.<br/> El valor por defecto es verdadero.|
| [is_multiple_item_selection_allowed](/cells/es/python-net/aspose.cells.pivot/pivotfield/is_multiple_item_selection_allowed) | indica si el campo puede tener varios elementos<br/>seleccionado en el campo de página<br/> El valor predeterminado es falso.|
| [is_repeat_item_labels](/cells/es/python-net/aspose.cells.pivot/pivotfield/is_repeat_item_labels) | indica si el campo puede repetir etiquetas de elementos<br/> El valor predeterminado es falso.|
| [is_include_new_items_in_filter](/cells/es/python-net/aspose.cells.pivot/pivotfield/is_include_new_items_in_filter) | indica si el campo puede incluir nuevos elementos en el filtro manual<br/> El valor predeterminado es falso.|
| [is_insert_page_breaks_between_items](/cells/es/python-net/aspose.cells.pivot/pivotfield/is_insert_page_breaks_between_items) | indica si el campo puede insertar saltos de página entre elementos<br/>insertar salto de página después de cada elemento<br/> El valor predeterminado es falso.|
| [show_all_items](/cells/es/python-net/aspose.cells.pivot/pivotfield/show_all_items) | Indica si se muestran todos los elementos del informe de tabla dinámica,<br/>incluso si no contienen datos de resumen.<br/>mostrar elementos sin datos<br/> El valor predeterminado es falso.|
| [non_auto_sort_default](/cells/es/python-net/aspose.cells.pivot/pivotfield/non_auto_sort_default) | Indica si una operación de clasificación que se aplicará a este campo dinámico es una operación de clasificación automática o una clasificación de datos simple.|
| [is_auto_sort](/cells/es/python-net/aspose.cells.pivot/pivotfield/is_auto_sort) | Indica si el campo de tabla dinámica especificado se ordena automáticamente.|
| [is_ascend_sort](/cells/es/python-net/aspose.cells.pivot/pivotfield/is_ascend_sort) | Indica si el campo de tabla dinámica especificado se ordena automáticamente de forma ascendente.|
| [auto_sort_field](/cells/es/python-net/aspose.cells.pivot/pivotfield/auto_sort_field) | Representa el índice de campo de clasificación automática.<br/> -1 significa PivotField en sí mismo, otros significan la posición de los campos de datos.|
| [is_auto_show](/cells/es/python-net/aspose.cells.pivot/pivotfield/is_auto_show) | Indica si el campo de tabla dinámica especificado se muestra automáticamente, solo válido para excel 2003.|
| [is_ascend_show](/cells/es/python-net/aspose.cells.pivot/pivotfield/is_ascend_show) | Indica si el campo de tabla dinámica especificado se muestra automáticamente de forma ascendente.|
| [auto_show_count](/cells/es/python-net/aspose.cells.pivot/pivotfield/auto_show_count) |Representar el número de elementos superiores o inferiores<br/> que se muestran automáticamente en el campo de tabla dinámica especificado.|
| [auto_show_field](/cells/es/python-net/aspose.cells.pivot/pivotfield/auto_show_field) | Representa el índice de campo de exhibición automática -1 significa PivotField en sí mismo.<br/> Debe ser el índice de los campos de datos.|
| [function](/cells/es/python-net/aspose.cells.pivot/pivotfield/function) | Representa la función utilizada para resumir el campo de datos de la tabla dinámica.|
| [data_display_format](/cells/es/python-net/aspose.cells.pivot/pivotfield/data_display_format) | Representa cómo mostrar los valores contenidos en un campo de datos.|
| [base_field_index](/cells/es/python-net/aspose.cells.pivot/pivotfield/base_field_index) | Representa el campo base para un cálculo personalizado.|
| [base_item_position](/cells/es/python-net/aspose.cells.pivot/pivotfield/base_item_position) | Representa el elemento en el campo base para un cálculo personalizado.<br/> Válido solo para campos de datos.<br/>Debido a que PivotItemPosition.Custom es solo para lectura, si necesita configurar PivotItemPosition.Custom,<br/> establezca el atributo PivotField.BaseItemIndex.|
| [base_item_index](/cells/es/python-net/aspose.cells.pivot/pivotfield/base_item_index) | Representa el elemento en el campo base para un cálculo personalizado.<br/> Válido solo para campos de datos.|
| [current_page_item](/cells/es/python-net/aspose.cells.pivot/pivotfield/current_page_item) | Representa el elemento de página actual que se muestra para el campo de página (válido solo para campos de página).|
| [number](/cells/es/python-net/aspose.cells.pivot/pivotfield/number) | Representa el formato de visualización integrado de números y fechas.|
| [insert_blank_row](/cells/es/python-net/aspose.cells.pivot/pivotfield/insert_blank_row) | Indica si se inserta una línea en blanco después de cada elemento.|
| [show_subtotal_at_top](/cells/es/python-net/aspose.cells.pivot/pivotfield/show_subtotal_at_top) | cuando ShowInOutlineForm es verdadero, muestra los subtotales en la parte superior de la lista de elementos en lugar de en la parte inferior|
| [show_in_outline_form](/cells/es/python-net/aspose.cells.pivot/pivotfield/show_in_outline_form) | Indica si el diseño de este campo en forma de esquema en la vista de tabla dinámica|
| [number_format](/cells/es/python-net/aspose.cells.pivot/pivotfield/number_format) |Representa el formato de visualización personalizado de números y fechas.|
| [items](/cells/es/python-net/aspose.cells.pivot/pivotfield/items) | Obtenga todos los artículos básicos;|
| [original_items](/cells/es/python-net/aspose.cells.pivot/pivotfield/original_items) | Obtenga los elementos básicos originales;|
| [item_count](/cells/es/python-net/aspose.cells.pivot/pivotfield/item_count) | Obtiene el recuento de elementos base de este campo dinámico.|
| [show_compact](/cells/es/python-net/aspose.cells.pivot/pivotfield/show_compact) | Indica si se muestran etiquetas del siguiente campo en la misma columna en la vista de tabla dinámica|


###  Métodos
| Método| Descripción|
| :- | :- |
| [hide_item(index, is_hidden)](/cells/es/python-net/aspose.cells.pivot/pivotfield/hide_item/#int-bool) | Establece si el PivotItem específico en un campo de datos está oculto.|
| [hide_item(item_value, is_hidden)](/cells/es/python-net/aspose.cells.pivot/pivotfield/hide_item/#str-bool) | Establece si el PivotItem específico en un campo de datos está oculto.|
| [get_pivot_filter_by_type(type)](/cells/es/python-net/aspose.cells.pivot/pivotfield/get_pivot_filter_by_type/#PivotFilterType) | Obtiene el filtro dinámico del campo dinámico por tipo|
| [get_pivot_filters()](/cells/es/python-net/aspose.cells.pivot/pivotfield/get_pivot_filters/#) | Obtiene los filtros dinámicos del campo dinámico.|
| [init_pivot_items()](/cells/es/python-net/aspose.cells.pivot/pivotfield/init_pivot_items/#) | Inicie los elementos pivote del campo pivote|
| [get_calculated_field_formula()](/cells/es/python-net/aspose.cells.pivot/pivotfield/get_calculated_field_formula/#) | Obtenga la cadena de fórmula del campo calculado especificado.|
| [set_subtotals(subtotal_type, shown)](/cells/es/python-net/aspose.cells.pivot/pivotfield/set_subtotals/#PivotFieldSubtotalType-bool) | Establece si el campo especificado muestra esos subtotales.|
| [get_subtotals(subtotal_type)](/cells/es/python-net/aspose.cells.pivot/pivotfield/get_subtotals/#PivotFieldSubtotalType) | Obtiene si el campo especificado muestra esos subtotales.|
| [is_hidden_item(index)](/cells/es/python-net/aspose.cells.pivot/pivotfield/is_hidden_item/#int) | Indica si el PivotItem específico está oculto.|
| [is_hidden_item_detail(index)](/cells/es/python-net/aspose.cells.pivot/pivotfield/is_hidden_item_detail/#int) | Indica si el PivotItem específico es un detalle oculto.|
| [hide_item_detail(index, is_hidden_detail)](/cells/es/python-net/aspose.cells.pivot/pivotfield/hide_item_detail/#int-bool) | Establece si el PivotItem específico en un campo dinámico es un detalle oculto.|
| [hide_detail(is_hidden_detail)](/cells/es/python-net/aspose.cells.pivot/pivotfield/hide_detail/#bool) | Establece si los PivotItems en un campo dinámico son detalles ocultos. Es decir, contraer/expandir este campo.|
| [add_calculated_item(name, formula)](/cells/es/python-net/aspose.cells.pivot/pivotfield/add_calculated_item/#str-str) |Agregue un elemento calculado al campo dinámico.|



###  Ejemplos

```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Change PivotField's attributes
rowField = pivot.row_fields[0]
rowField.display_name = "custom display name"
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Ver también
* módulo [aspose.cells.pivot](..)
