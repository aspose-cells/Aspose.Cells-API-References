---
title: Cell clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 140
url: /es/python-net/aspose.cells/cell/
is_root: false
---
##  Cell clase
Encapsula el objeto que representa una única celda de Workbook.



El tipo Cell expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [worksheet](/cells/es/python-net/aspose.cells/cell/worksheet) | Obtiene la hoja de cálculo principal.|
| [date_time_value](/cells/es/python-net/aspose.cells/cell/date_time_value) | Obtiene el valor DateTime contenido en la celda.|
| [row](/cells/es/python-net/aspose.cells/cell/row) | Obtiene el número de fila (basado en cero) de la celda.|
| [column](/cells/es/python-net/aspose.cells/cell/column) | Obtiene el número de columna (basado en cero) de la celda.|
| [is_formula](/cells/es/python-net/aspose.cells/cell/is_formula) | Representa si la celda especificada contiene fórmula.|
| [type](/cells/es/python-net/aspose.cells/cell/type) | Representa el tipo de valor de celda.|
| [name](/cells/es/python-net/aspose.cells/cell/name) | Obtiene el nombre de la celda.|
| [is_error_value](/cells/es/python-net/aspose.cells/cell/is_error_value) | Comprueba si el valor de esta celda es un error.|
| [is_numeric_value](/cells/es/python-net/aspose.cells/cell/is_numeric_value) | Indica si el valor interno de esta celda es numérico (int, double y datetime)|
| [string_value](/cells/es/python-net/aspose.cells/cell/string_value) |Obtiene el valor de cadena contenido en la celda. Si el tipo de esta celda es una cadena, devuelva el valor de la cadena en sí.<br/>Para otros tipos de celdas, se devolverá el valor de cadena con formato (formateado con el estilo especificado de esta celda).<br/>El valor de la celda con formato es el mismo que puede obtener de Excel al copiar una celda como texto (como<br/> copiando la celda al editor de texto o exportando a csv).|
| [string_value_without_format](/cells/es/python-net/aspose.cells/cell/string_value_without_format) | Obtiene el valor de la celda como cadena sin ningún formato.|
| [number_category_type](/cells/es/python-net/aspose.cells/cell/number_category_type) | Representa el tipo de categoría del formato de número de esta celda.|
| [display_string_value](/cells/es/python-net/aspose.cells/cell/display_string_value) | Obtiene el valor de cadena con formato de esta celda según el estilo de visualización de la celda.|
| [int_value](/cells/es/python-net/aspose.cells/cell/int_value) | Obtiene el valor entero contenido en la celda.|
| [double_value](/cells/es/python-net/aspose.cells/cell/double_value) | Obtiene el valor doble contenido en la celda.|
| [float_value](/cells/es/python-net/aspose.cells/cell/float_value) | Obtiene el valor flotante contenido en la celda.|
| [bool_value](/cells/es/python-net/aspose.cells/cell/bool_value) | Obtiene el valor booleano contenido en la celda.|
| [has_custom_style](/cells/es/python-net/aspose.cells/cell/has_custom_style) | Indica si esta celda tiene una configuración de estilo personalizada (diferente a la predeterminada heredada)<br/> de la fila, columna o libro de trabajo correspondiente).|
| [shared_style_index](/cells/es/python-net/aspose.cells/cell/shared_style_index) | Obtiene el índice de estilo compartido de la celda en el grupo de estilos.|
| [formula](/cells/es/python-net/aspose.cells/cell/formula) | Obtiene o establece una fórmula de [Cell](/cells/es/python-net/aspose.cells/cell).|
| [formula_local](/cells/es/python-net/aspose.cells/cell/formula_local) | Obtenga la fórmula con formato de configuración regional de la celda.|
| [r1c1_formula](/cells/es/python-net/aspose.cells/cell/r1c1_formula) | Obtiene o establece una fórmula R1C1 de [Cell](/cells/es/python-net/aspose.cells/cell).|
| [contains_external_link](/cells/es/python-net/aspose.cells/cell/contains_external_link) |Indica si esta celda contiene un enlace externo.<br/> Solo se aplica cuando la celda es una celda de fórmula.|
| [is_array_header](/cells/es/python-net/aspose.cells/cell/is_array_header) | Indica que la fórmula de la celda es una fórmula matricial<br/> y es la primera celda de la matriz.|
| [is_dynamic_array_formula](/cells/es/python-net/aspose.cells/cell/is_dynamic_array_formula) | Indica si la fórmula de la celda es una fórmula de matriz dinámica (verdadera) o una fórmula de matriz heredada (falsa).|
| [is_array_formula](/cells/es/python-net/aspose.cells/cell/is_array_formula) | Indica si la fórmula de la celda es una fórmula matricial.|
| [is_in_array](/cells/es/python-net/aspose.cells/cell/is_in_array) | Indica si la fórmula de la celda es una fórmula matricial.|
| [is_shared_formula](/cells/es/python-net/aspose.cells/cell/is_shared_formula) | Indica si la fórmula de la celda forma parte de una fórmula compartida.|
| [is_table_formula](/cells/es/python-net/aspose.cells/cell/is_table_formula) | Indica si esta celda es parte de la fórmula de la tabla.|
| [is_in_table](/cells/es/python-net/aspose.cells/cell/is_in_table) | Indica si esta celda es parte de la fórmula de la tabla.|
| [value](/cells/es/python-net/aspose.cells/cell/value) | Obtiene el valor contenido en esta celda.|
| [is_style_set](/cells/es/python-net/aspose.cells/cell/is_style_set) | Indica si el estilo de la celda está establecido. Si devuelve falso, significa que esta celda tiene un formato de celda predeterminado.|
| [is_merged](/cells/es/python-net/aspose.cells/cell/is_merged) | Comprueba si una celda es parte de un rango combinado o no.|
| [comment](/cells/es/python-net/aspose.cells/cell/comment) | Obtiene el comentario de esta celda.|
| [html_string](/cells/es/python-net/aspose.cells/cell/html_string) | Obtiene y establece la cadena html que contiene datos y algunos formatos en esta celda.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [calculate(options)](/cells/es/python-net/aspose.cells/cell/calculate/#CalculationOptions) | Calcula la fórmula de la celda.|
| [calculate(ignore_error, custom_function)](/cells/es/python-net/aspose.cells/cell/calculate/#bool-ICustomFunction) | Calcula la fórmula de la celda.|
| [put_value(bool_value)](/cells/es/python-net/aspose.cells/cell/put_value/#bool) | Pone un valor booleano en la celda.|
| [put_value(int_value)](/cells/es/python-net/aspose.cells/cell/put_value/#int) | Pone un valor entero en la celda.|
| [put_value(double_value)](/cells/es/python-net/aspose.cells/cell/put_value/#float) |Pone un valor doble en la celda.|
| [put_value(string_value, is_converted, set_style)](/cells/es/python-net/aspose.cells/cell/put_value/#str-bool-bool) | Pone un valor en la celda, si corresponde, el valor se convertirá a otro tipo de datos y el formato de número de la celda se restablecerá.|
| [put_value(string_value, is_converted)](/cells/es/python-net/aspose.cells/cell/put_value/#str-bool) | Coloca un valor de cadena en la celda y convierte el valor a otro tipo de datos, si corresponde.|
| [put_value(string_value)](/cells/es/python-net/aspose.cells/cell/put_value/#str) | Pone un valor de cadena en la celda.|
| [put_value(date_time)](/cells/es/python-net/aspose.cells/cell/put_value/#DateTime) | Pone un valor DateTime en la celda.|
| [put_value(object_value)](/cells/es/python-net/aspose.cells/cell/put_value/#any) | Pone un valor de objeto en la celda.|
| [get_display_style()](/cells/es/python-net/aspose.cells/cell/get_display_style/#) | Obtiene el estilo de visualización de la celda.<br/>Si esta celda también se ve afectada por otras configuraciones, como el formato condicional, la lista de objetos, etc.,<br/> entonces el estilo de visualización puede ser diferente de cell.GetStyle().|
| [get_display_style(include_merged_borders)](/cells/es/python-net/aspose.cells/cell/get_display_style/#bool) | Obtiene el estilo de visualización de la celda.<br/> Si la celda tiene formato condicional, el estilo de visualización no es el mismo que el de cell.GetStyle().|
| [get_style()](/cells/es/python-net/aspose.cells/cell/get_style/#) | Obtiene el estilo de celda.|
| [get_style(check_borders)](/cells/es/python-net/aspose.cells/cell/get_style/#bool) | Si checkBorders es verdadero, verifica si los bordes de otras celdas afectarán el estilo de esta celda.|
| [set_style(style)](/cells/es/python-net/aspose.cells/cell/set_style/#Style) | Establece el estilo de celda.|
| [set_style(style, explicit_flag)](/cells/es/python-net/aspose.cells/cell/set_style/#Style-bool) | Aplicar el estilo de celda.|
| [set_style(style, flag)](/cells/es/python-net/aspose.cells/cell/set_style/#Style-StyleFlag) | Aplicar el estilo de celda.|
| [set_formula(formula, value)](/cells/es/python-net/aspose.cells/cell/set_formula/#str-any) | Establezca la fórmula y el valor de la fórmula.|
| [set_formula(formula, is_r1c1, is_local, value)](/cells/es/python-net/aspose.cells/cell/set_formula/#str-bool-bool-any) | Establezca la fórmula y el valor de la fórmula.|
| [set_formula(formula, options, value)](/cells/es/python-net/aspose.cells/cell/set_formula/#str-FormulaParseOptions-any) | Establezca la fórmula y el valor de la fórmula.|
| [set_array_formula(array_formula, row_number, column_number, is_r1c1, is_local)](/cells/es/python-net/aspose.cells/cell/set_array_formula/#str-int-int-bool-bool) | Establece una fórmula de matriz en un rango de celdas.|
| [set_array_formula(array_formula, row_number, column_number)](/cells/es/python-net/aspose.cells/cell/set_array_formula/#str-int-int) |Establece una fórmula de matriz (fórmula de matriz heredada ingresada mediante CTRL+MAYÚS+ENTRAR en MS Excel) en un rango de celdas.|
| [set_array_formula(array_formula, row_number, column_number, options)](/cells/es/python-net/aspose.cells/cell/set_array_formula/#str-int-int-FormulaParseOptions) | Establece una fórmula de matriz en un rango de celdas.|
| [set_array_formula(array_formula, row_number, column_number, options, values)](/cells/es/python-net/aspose.cells/cell/set_array_formula/#str-int-int-FormulaParseOptions-list) | Establece una fórmula de matriz en un rango de celdas.|
| [set_shared_formula(shared_formula, row_number, column_number, is_r1c1, is_local)](/cells/es/python-net/aspose.cells/cell/set_shared_formula/#str-int-int-bool-bool) | Establece una fórmula para un rango de celdas.|
| [set_shared_formula(shared_formula, row_number, column_number)](/cells/es/python-net/aspose.cells/cell/set_shared_formula/#str-int-int) | Establece fórmulas compartidas en un rango de celdas.|
| [set_shared_formula(shared_formula, row_number, column_number, options)](/cells/es/python-net/aspose.cells/cell/set_shared_formula/#str-int-int-FormulaParseOptions) | Establece fórmulas compartidas en un rango de celdas.|
| [set_shared_formula(shared_formula, row_number, column_number, options, values)](/cells/es/python-net/aspose.cells/cell/set_shared_formula/#str-int-int-FormulaParseOptions-list) | Establece fórmulas compartidas en un rango de celdas.|
| [get_leafs()](/cells/es/python-net/aspose.cells/cell/get_leafs/#) | Obtenga todas las celdas que hacen referencia a esta celda directamente y deben actualizarse cuando se modifica esta celda.|
| [get_leafs(recursive)](/cells/es/python-net/aspose.cells/cell/get_leafs/#bool) | Obtenga todas las celdas que se actualizarán cuando se modifique esta celda.|
| [set_dynamic_array_formula(array_formula, options, calculate_value)](/cells/es/python-net/aspose.cells/cell/set_dynamic_array_formula/#str-FormulaParseOptions-bool) | Establece la fórmula de matriz dinámica y hace que la fórmula se derrame en las celdas vecinas si es posible.|
| [set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value)](/cells/es/python-net/aspose.cells/cell/set_dynamic_array_formula/#str-FormulaParseOptions-list-bool-bool) | Establece la fórmula de matriz dinámica y hace que la fórmula se derrame en las celdas vecinas si es posible.|
| [set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value, copts)](/cells/es/python-net/aspose.cells/cell/set_dynamic_array_formula/#str-FormulaParseOptions-list-bool-bool-CalculationOptions) | Establece la fórmula de matriz dinámica y hace que la fórmula se derrame en las celdas vecinas si es posible.|
| [set_table_formula(row_number, column_number, row_input_cell, column_input_cell, values)](/cells/es/python-net/aspose.cells/cell/set_table_formula/#int-int-str-str-list) | Cree una tabla de datos de dos variables para el rango dado a partir de esta celda.|
| [set_table_formula(row_number, column_number, input_cell, is_row_input, values)](/cells/es/python-net/aspose.cells/cell/set_table_formula/#int-int-str-bool-list) | Cree una tabla de datos de una variable para el rango dado a partir de esta celda.|
| [set_table_formula(row_number, column_number, row_index_of_row_input_cell, column_index_of_row_input_cell, row_index_of_column_input_cell, column_index_of_column_input_cell, values)](/cells/es/python-net/aspose.cells/cell/set_table_formula/#int-int-int-int-int-int-list) | Cree una tabla de datos de dos variables para el rango dado a partir de esta celda.|
| [set_table_formula(row_number, column_number, row_index_of_input_cell, column_index_of_input_cell, is_row_input, values)](/cells/es/python-net/aspose.cells/cell/set_table_formula/#int-int-int-int-bool-list) | Cree una tabla de datos de una variable para el rango dado a partir de esta celda.|
| [get_characters()](/cells/es/python-net/aspose.cells/cell/get_characters/#) | Devuelve todos los objetos de caracteres.<br/> que representa un rango de caracteres dentro del texto de la celda.|
| [get_characters(flag)](/cells/es/python-net/aspose.cells/cell/get_characters/#bool) | Devuelve todos los objetos de caracteres.<br/> que representa un rango de caracteres dentro del texto de la celda.|
| [get_string_value(format_strategy)](/cells/es/python-net/aspose.cells/cell/get_string_value/#CellValueFormatStrategy) | Obtiene el valor de cadena por estrategia de formato específica.|
| [get_width_of_value()](/cells/es/python-net/aspose.cells/cell/get_width_of_value/#) | Obtiene el ancho del valor en unidades de píxeles.|
| [get_height_of_value()](/cells/es/python-net/aspose.cells/cell/get_height_of_value/#) | Obtiene el alto del valor en unidades de píxeles.|
| [get_format_conditions()](/cells/es/python-net/aspose.cells/cell/get_format_conditions/#) | Obtiene las condiciones de formato que se aplican a esta celda.|
| [get_formula(is_r1c1, is_local)](/cells/es/python-net/aspose.cells/cell/get_formula/#bool-bool) | Obtenga la fórmula de esta celda.|
| [get_precedents()](/cells/es/python-net/aspose.cells/cell/get_precedents/#) |Obtiene todas las referencias que aparecen en la fórmula de esta celda.|
| [get_dependents(is_all)](/cells/es/python-net/aspose.cells/cell/get_dependents/#bool) | Obtenga todas las celdas cuya fórmula hace referencia directamente a esta celda.|
| [get_precedents_in_calculation()](/cells/es/python-net/aspose.cells/cell/get_precedents_in_calculation/#) | Obtiene todos los precedentes (referencia a celdas en el libro de trabajo actual) usados por la fórmula de esta celda mientras se calcula.|
| [get_dependents_in_calculation(recursive)](/cells/es/python-net/aspose.cells/cell/get_dependents_in_calculation/#bool) | Obtiene todas las celdas cuyo resultado calculado depende de esta celda.|
| [get_array_range()](/cells/es/python-net/aspose.cells/cell/get_array_range/#) | Obtiene el rango de matriz si la fórmula de la celda es una fórmula de matriz.|
| [remove_array_formula(leave_normal_formula)](/cells/es/python-net/aspose.cells/cell/remove_array_formula/#bool) | Eliminar fórmula matricial.|
| [copy(cell)](/cells/es/python-net/aspose.cells/cell/copy/#Cell) | Copia datos de una celda de origen.|
| [characters(start_index, length)](/cells/es/python-net/aspose.cells/cell/characters/#int-int) | Devuelve un objeto Characters que representa un rango de caracteres dentro del texto de la celda.|
| [is_rich_text()](/cells/es/python-net/aspose.cells/cell/is_rich_text/#) | Indica si el valor de la cadena de celdas es un texto enriquecido.|
| [set_characters(characters)](/cells/es/python-net/aspose.cells/cell/set_characters/#list) | Establece el formato de texto enriquecido de la celda.|
| [get_merged_range()](/cells/es/python-net/aspose.cells/cell/get_merged_range/#) | Devuelve un objeto [Range](/cells/es/python-net/aspose.cells/range) que representa un rango combinado.|
| [get_html_string(html5)](/cells/es/python-net/aspose.cells/cell/get_html_string/#bool) | Obtiene la cadena html que contiene datos y algunos formatos en esta celda.|
| [to_json()](/cells/es/python-net/aspose.cells/cell/to_json/#) | Convierta [Cell](/cells/es/python-net/aspose.cells/cell) a JSON datos de estructura.|
| [equals(cell)](/cells/es/python-net/aspose.cells/cell/equals/#Cell) | Comprueba si este objeto hace referencia a la misma celda con otro objeto de celda.|
| [get_conditional_formatting_result()](/cells/es/python-net/aspose.cells/cell/get_conditional_formatting_result/#) | Obtenga el resultado del formato condicional.|
| [get_validation()](/cells/es/python-net/aspose.cells/cell/get_validation/#) |Obtiene la validación aplicada a esta celda.|
| [get_validation_value()](/cells/es/python-net/aspose.cells/cell/get_validation_value/#) | Obtiene el valor de validación que se aplicó a esta celda.|
| [get_table()](/cells/es/python-net/aspose.cells/cell/get_table/#) | Obtiene la tabla que contiene esta celda.|



###  Ejemplo

```python
from aspose.cells import TextAlignmentType, Workbook
from aspose.pydrawing import Color

excel = Workbook()
cells = excel.worksheets[0].cells
# Put a string into a cell
cell = cells.get(0, 0)
cell.put_value("Hello")
first = cell.string_value
# Put an integer into a cell
cell = cells.get("B1")
cell.put_value(12)
second = cell.int_value
# Put a double into a cell
cell = cells.get(0, 2)
cell.put_value(-1.234)
third = cell.double_value
# Put a formula into a cell
cell = cells.get("D1")
cell.formula = "=B1 + C1"
# Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
cell = cells.get("b2")
cell.formula = "=sum(average(b1,c1), b1)"
# Set style of a cell
style = cell.get_style()
# Set background color
style.background_color = Color.yellow
# Set format of a cell
style.font.name = "Courier New"
style.vertical_alignment = TextAlignmentType.TOP
cell.set_style(style)

```

###  Ver también
* módulo [aspose.cells](..)
* clase [Cell](/cells/es/python-net/aspose.cells/cell)
* clase [Range](/cells/es/python-net/aspose.cells/range)
