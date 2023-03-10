---
title: Cells clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 180
url: /es/python-net/aspose.cells/cells/
is_root: false
---
##  Cells clase
Encapsula una colección de objetos relevantes para celdas, como [Cell](/cells/es/python-net/aspose.cells/cell), [Row](/cells/es/python-net/aspose.cells/row), etc.



El tipo Cells expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [ods_cell_fields](/cells/es/python-net/aspose.cells/cells/ods_cell_fields) | Obtiene la lista de campos de ods.|
| [count](/cells/es/python-net/aspose.cells/cells/count) | Obtiene el recuento total de objetos Cell instanciados.|
| [count_large](/cells/es/python-net/aspose.cells/cells/count_large) | Obtiene el recuento total de objetos Cell instanciados.|
| [rows](/cells/es/python-net/aspose.cells/cells/rows) | Obtiene la colección de objetos [Row](/cells/es/python-net/aspose.cells/row) que representa las filas individuales de esta hoja de trabajo.|
| [merged_cells](/cells/es/python-net/aspose.cells/cells/merged_cells) | Obtiene la colección de celdas combinadas.|
| [multi_thread_reading](/cells/es/python-net/aspose.cells/cells/multi_thread_reading) | Obtiene o establece si el modelo de datos de las celdas debe admitir la lectura de subprocesos múltiples.<br/> El valor predeterminado de esta propiedad es falso.|
| [memory_setting](/cells/es/python-net/aspose.cells/cells/memory_setting) | Obtiene o establece la opción de uso de memoria para estas celdas.|
| [style](/cells/es/python-net/aspose.cells/cells/style) | Obtiene y establece el estilo predeterminado.|
| [standard_width_inch](/cells/es/python-net/aspose.cells/cells/standard_width_inch) |Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de pulgadas.|
| [standard_width_pixels](/cells/es/python-net/aspose.cells/cells/standard_width_pixels) | Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de píxeles.|
| [standard_width](/cells/es/python-net/aspose.cells/cells/standard_width) | Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de caracteres.|
| [standard_height](/cells/es/python-net/aspose.cells/cells/standard_height) | Obtiene o establece el alto de fila predeterminado en esta hoja de cálculo, en unidades de puntos.|
| [standard_height_pixels](/cells/es/python-net/aspose.cells/cells/standard_height_pixels) | Obtiene o establece el alto de fila predeterminado en esta hoja de cálculo, en unidades de píxeles.|
| [standard_height_inch](/cells/es/python-net/aspose.cells/cells/standard_height_inch) | Obtiene o establece el alto de fila predeterminado en esta hoja de cálculo, en unidades de pulgadas.|
| [preserve_string](/cells/es/python-net/aspose.cells/cells/preserve_string) | Obtiene o establece un valor que indica si todos los valores de la hoja de cálculo se conservan como cadenas.<br/> El valor predeterminado es falso.|
| [min_row](/cells/es/python-net/aspose.cells/cells/min_row) | Índice de fila mínimo de celda que contiene datos o estilo.|
| [max_row](/cells/es/python-net/aspose.cells/cells/max_row) | Índice de fila máximo de celda que contiene datos o estilo.|
| [min_column](/cells/es/python-net/aspose.cells/cells/min_column) | Índice de columna mínimo de aquellas celdas que se han instanciado en la colección (no incluye la columna<br/> donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda).|
| [max_column](/cells/es/python-net/aspose.cells/cells/max_column) | Índice de columna mínimo de aquellas celdas que se han instanciado en la colección (no incluye la columna<br/> donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda).|
| [min_data_row](/cells/es/python-net/aspose.cells/cells/min_data_row) | Índice de fila mínimo de celda que contiene datos.|
| [max_data_row](/cells/es/python-net/aspose.cells/cells/max_data_row) |Índice de fila máximo de celda que contiene datos.|
| [min_data_column](/cells/es/python-net/aspose.cells/cells/min_data_column) | Índice de columna mínimo de la celda que contiene datos.|
| [max_data_column](/cells/es/python-net/aspose.cells/cells/max_data_column) | Índice de columna máximo de celda que contiene datos.|
| [is_default_row_height_matched](/cells/es/python-net/aspose.cells/cells/is_default_row_height_matched) | Indica que la altura de fila y la altura de fuente predeterminada coinciden|
| [is_default_row_hidden](/cells/es/python-net/aspose.cells/cells/is_default_row_hidden) | Indica si la fila está oculta de forma predeterminada.|
| [columns](/cells/es/python-net/aspose.cells/cells/columns) | Obtiene la colección de objetos [Column](/cells/es/python-net/aspose.cells/column) que representa las columnas individuales de esta hoja de cálculo.|
| [ranges](/cells/es/python-net/aspose.cells/cells/ranges) | Obtiene la colección de objetos [Range](/cells/es/python-net/aspose.cells/range) creados en tiempo de ejecución.|
| [last_cell](/cells/es/python-net/aspose.cells/cells/last_cell) | Obtiene la última celda de esta hoja de cálculo.|
| [max_display_range](/cells/es/python-net/aspose.cells/cells/max_display_range) | Obtiene el rango máximo que incluye datos, celdas combinadas y formas.|
| [first_cell](/cells/es/python-net/aspose.cells/cells/first_cell) | Obtiene la primera celda de esta hoja de cálculo.|



Obtiene el elemento [Cell](/cells/es/python-net/aspose.cells/cell) dentro de la hoja de trabajo
###  indexador
| Nombre| Descripción|
| :- | :- |
| [index] | El índice de base cero del elemento.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [create_range(upper_left_cell, lower_right_cell)](/cells/es/python-net/aspose.cells/cells/create_range/#str-str) | Crea un objeto [Range](/cells/es/python-net/aspose.cells/range) a partir de un rango de celdas.|
| [create_range(first_row, first_column, total_rows, total_columns)](/cells/es/python-net/aspose.cells/cells/create_range/#int-int-int-int) | Crea un objeto [Range](/cells/es/python-net/aspose.cells/range) a partir de un rango de celdas.|
| [create_range(address)](/cells/es/python-net/aspose.cells/cells/create_range/#str) | Crea un objeto [Range](/cells/es/python-net/aspose.cells/range) a partir de una dirección del rango.|
| [create_range(first_index, number, is_vertical)](/cells/es/python-net/aspose.cells/cells/create_range/#int-int-bool) | Crea un objeto [Range](/cells/es/python-net/aspose.cells/range) a partir de filas de celdas o columnas de celdas.|
| [get(row, column)](/cells/es/python-net/aspose.cells/cells/get/#int-int) |Agregue API for Python a través de .Net.ya que esta [fila int, columna int] no es compatible|
| [get(cell_name)](/cells/es/python-net/aspose.cells/cells/get/#str) | Agregue API for Python a través de .Net.ya que este [string cellName] no es compatible|
| [import_object_array(obj_array, first_row, first_column, is_vertical)](/cells/es/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool) | Importa una matriz de datos en una hoja de trabajo.|
| [import_object_array(obj_array, first_row, first_column, is_vertical, skip)](/cells/es/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool-int) | Importa una matriz de datos en una hoja de trabajo.|
| [import_array(string_array, first_row, first_column, is_vertical)](/cells/es/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Importa una matriz de cadenas en una hoja de cálculo.|
| [import_array(int_array, first_row, first_column, is_vertical)](/cells/es/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Importa una matriz de enteros en una hoja de cálculo.|
| [import_array(double_array, first_row, first_column, is_vertical)](/cells/es/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Importa una matriz de doble en una hoja de trabajo.|
| [import_csv(file_name, splitter, convert_numeric_data, first_row, first_column)](/cells/es/python-net/aspose.cells/cells/import_csv/#str-str-bool-int-int) | Importe un archivo CSV a las celdas.|
| [import_csv(stream, splitter, convert_numeric_data, first_row, first_column)](/cells/es/python-net/aspose.cells/cells/import_csv/#io.RawIOBase-str-bool-int-int) | Importe un archivo CSV a las celdas.|
| [import_csv(file_name, options, first_row, first_column)](/cells/es/python-net/aspose.cells/cells/import_csv/#str-TxtLoadOptions-int-int) | Importe un archivo CSV a las celdas.|
| [import_csv(stream, options, first_row, first_column)](/cells/es/python-net/aspose.cells/cells/import_csv/#io.RawIOBase-TxtLoadOptions-int-int) | Importe un archivo CSV a las celdas.|
| [merge(first_row, first_column, total_rows, total_columns)](/cells/es/python-net/aspose.cells/cells/merge/#int-int-int-int) | Combina un rango específico de celdas en una sola celda.|
| [merge(first_row, first_column, total_rows, total_columns, merge_conflict)](/cells/es/python-net/aspose.cells/cells/merge/#int-int-int-int-bool) | Combina un rango específico de celdas en una sola celda.|
| [merge(first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict)](/cells/es/python-net/aspose.cells/cells/merge/#int-int-int-int-bool-bool) | Combina un rango específico de celdas en una sola celda.|
| [copy_columns(source_cells0, source_column_index, destination_column_index, column_number, paste_options)](/cells/es/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int-PasteOptions) | Copia datos y formatos de una columna completa.|
| [copy_columns(source_cells0, source_column_index, destination_column_index, column_number)](/cells/es/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int) | Copia datos y formatos de una columna completa.|
| [copy_columns(source_cells, source_column_index, source_total_columns, destination_column_index, destination_total_columns)](/cells/es/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int-int) | Copia datos y formatos de las columnas enteras.|
| [copy_rows(source_cells, source_row_index, destination_row_index, row_number)](/cells/es/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int) | Copia datos y formatos de algunas filas completas.|
| [copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options)](/cells/es/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int-CopyOptions) | Copia datos y formatos de algunas filas completas.|
| [copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options, paste_options)](/cells/es/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int-CopyOptions-PasteOptions) | Copia datos y formatos de algunas filas completas.|
| [group_columns(first_index, last_index)](/cells/es/python-net/aspose.cells/cells/group_columns/#int-int) | Columnas de grupos.|
| [group_columns(first_index, last_index, is_hidden)](/cells/es/python-net/aspose.cells/cells/group_columns/#int-int-bool) | Columnas de grupos.|
| [ungroup_rows(first_index, last_index, is_all)](/cells/es/python-net/aspose.cells/cells/ungroup_rows/#int-int-bool) | Desagrupa filas.|
| [ungroup_rows(first_index, last_index)](/cells/es/python-net/aspose.cells/cells/ungroup_rows/#int-int) | Desagrupa filas.|
| [group_rows(first_index, last_index, is_hidden)](/cells/es/python-net/aspose.cells/cells/group_rows/#int-int-bool) | Agrupa filas.|
| [group_rows(first_index, last_index)](/cells/es/python-net/aspose.cells/cells/group_rows/#int-int) | Agrupa filas.|
| [delete_column(column_index, update_reference)](/cells/es/python-net/aspose.cells/cells/delete_column/#int-bool) | Elimina una columna.|
| [delete_column(column_index)](/cells/es/python-net/aspose.cells/cells/delete_column/#int) | Elimina una columna.|
| [delete_rows(row_index, total_rows)](/cells/es/python-net/aspose.cells/cells/delete_rows/#int-int) | Elimina varias filas.|
| [delete_rows(row_index, total_rows, update_reference)](/cells/es/python-net/aspose.cells/cells/delete_rows/#int-int-bool) | Elimina varias filas en la hoja de cálculo.|
| [delete_blank_columns()](/cells/es/python-net/aspose.cells/cells/delete_blank_columns/#) | Elimine todas las columnas en blanco que no contengan ningún dato.|
| [delete_blank_columns(options)](/cells/es/python-net/aspose.cells/cells/delete_blank_columns/#DeleteOptions) | Elimine todas las columnas en blanco que no contengan ningún dato.|
| [delete_blank_rows()](/cells/es/python-net/aspose.cells/cells/delete_blank_rows/#) | Elimine todas las filas en blanco que no contengan ningún dato.|
| [delete_blank_rows(options)](/cells/es/python-net/aspose.cells/cells/delete_blank_rows/#DeleteOptions) | Elimine todas las filas en blanco que no contengan ningún dato.|
| [insert_columns(column_index, total_columns)](/cells/es/python-net/aspose.cells/cells/insert_columns/#int-int) | Inserta algunas columnas en la hoja de trabajo.|
| [insert_columns(column_index, total_columns, update_reference)](/cells/es/python-net/aspose.cells/cells/insert_columns/#int-int-bool) | Inserta algunas columnas en la hoja de trabajo.|
| [insert_column(column_index, update_reference)](/cells/es/python-net/aspose.cells/cells/insert_column/#int-bool) |Inserta una nueva columna en la hoja de cálculo.|
| [insert_column(column_index)](/cells/es/python-net/aspose.cells/cells/insert_column/#int) |Inserta una nueva columna en la hoja de cálculo.|
| [insert_rows(row_index, total_rows, update_reference)](/cells/es/python-net/aspose.cells/cells/insert_rows/#int-int-bool) | Inserta varias filas en la hoja de cálculo.|
| [insert_rows(row_index, total_rows, options)](/cells/es/python-net/aspose.cells/cells/insert_rows/#int-int-InsertOptions) | Inserta varias filas en la hoja de cálculo.|
| [insert_rows(row_index, total_rows)](/cells/es/python-net/aspose.cells/cells/insert_rows/#int-int) | Inserta varias filas en la hoja de cálculo.|
| [clear_range(range)](/cells/es/python-net/aspose.cells/cells/clear_range/#CellArea) | Borra el contenido y el formato de un rango.|
| [clear_range(start_row, start_column, end_row, end_column)](/cells/es/python-net/aspose.cells/cells/clear_range/#int-int-int-int) | Borra el contenido y el formato de un rango.|
| [clear_contents(range)](/cells/es/python-net/aspose.cells/cells/clear_contents/#CellArea) | Borra el contenido de un rango.|
| [clear_contents(start_row, start_column, end_row, end_column)](/cells/es/python-net/aspose.cells/cells/clear_contents/#int-int-int-int) | Borra el contenido de un rango.|
| [clear_formats(range)](/cells/es/python-net/aspose.cells/cells/clear_formats/#CellArea) | Borra el formato de un rango.|
| [clear_formats(start_row, start_column, end_row, end_column)](/cells/es/python-net/aspose.cells/cells/clear_formats/#int-int-int-int) | Borra el formato de un rango.|
| [find(what, previous_cell)](/cells/es/python-net/aspose.cells/cells/find/#any-Cell) | Encuentra la celda que contiene el objeto de entrada.|
| [find(what, previous_cell, find_options)](/cells/es/python-net/aspose.cells/cells/find/#any-Cell-FindOptions) | Encuentra la celda que contiene el objeto de entrada.|
| [end_cell_in_row(row_index)](/cells/es/python-net/aspose.cells/cells/end_cell_in_row/#int) | Obtiene la última celda de esta fila.|
| [end_cell_in_row(start_row, end_row, start_column, end_column)](/cells/es/python-net/aspose.cells/cells/end_cell_in_row/#int-int-int-int) | Obtiene la última celda con el índice de fila máximo en este rango.|
| [end_cell_in_column(column_index)](/cells/es/python-net/aspose.cells/cells/end_cell_in_column/#int) | Obtiene la última celda de esta columna.|
| [end_cell_in_column(start_row, end_row, start_column, end_column)](/cells/es/python-net/aspose.cells/cells/end_cell_in_column/#int-int-int-int) | Obtiene la última celda con el índice de columna máximo en este rango.|
| [insert_range(area, shift_number, shift_type, update_reference)](/cells/es/python-net/aspose.cells/cells/insert_range/#CellArea-int-ShiftType-bool) | Inserta un rango de celdas y desplaza celdas según la opción de desplazamiento.|
| [insert_range(area, shift_type)](/cells/es/python-net/aspose.cells/cells/insert_range/#CellArea-ShiftType) | Inserta un rango de celdas y desplaza celdas según la opción de desplazamiento.|
| [insert_range(area, shift_number, shift_type)](/cells/es/python-net/aspose.cells/cells/insert_range/#CellArea-int-ShiftType) | Inserta un rango de celdas y desplaza celdas según la opción de desplazamiento.|
| [import_custom_objects(list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number)](/cells/es/python-net/aspose.cells/cells/import_custom_objects/#list-list-bool-int-int-int-bool-str-bool) | Importa objetos personalizados.|
| [import_custom_objects(list, first_row, first_column, options)](/cells/es/python-net/aspose.cells/cells/import_custom_objects/#list-int-int-ImportTableOptions) | Importa objetos personalizados.|
| [subtotal(ca, group_by, function, total_list)](/cells/es/python-net/aspose.cells/cells/subtotal/#CellArea-int-ConsolidationFunction-list) | Crea subtotales para el rango.|
| [subtotal(ca, group_by, function, total_list, replace, page_breaks, summary_below_data)](/cells/es/python-net/aspose.cells/cells/subtotal/#CellArea-int-ConsolidationFunction-list-bool-bool-bool) | Crea subtotales para el rango.|
| [remove_duplicates()](/cells/es/python-net/aspose.cells/cells/remove_duplicates/#) | Elimina filas duplicadas en la hoja.|
| [remove_duplicates(start_row, start_column, end_row, end_column)](/cells/es/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int) | Elimina valores duplicados en el rango.|
| [remove_duplicates(start_row, start_column, end_row, end_column, has_headers, column_offsets)](/cells/es/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int-bool-list) | Elimina los datos duplicados del rango.|
| [get_row_enumerator()](/cells/es/python-net/aspose.cells/cells/get_row_enumerator/#) | Obtiene el enumerador de filas.|
| [get_cell(row, column)](/cells/es/python-net/aspose.cells/cells/get_cell/#int-int) | Obtiene el elemento [Cell](/cells/es/python-net/aspose.cells/cell) o nulo en el índice de fila de celda y el índice de columna especificados.|
| [get_row(row)](/cells/es/python-net/aspose.cells/cells/get_row/#int) | Obtiene el elemento [Row](/cells/es/python-net/aspose.cells/row) en el índice de fila de celda especificado.|
| [check_cell(row, column)](/cells/es/python-net/aspose.cells/cells/check_cell/#int-int) | Obtiene el elemento [Cell](/cells/es/python-net/aspose.cells/cell) o nulo en el índice de fila de celda y el índice de columna especificados.|
| [check_row(row)](/cells/es/python-net/aspose.cells/cells/check_row/#int) |Obtiene el elemento [Row](/cells/es/python-net/aspose.cells/row) o en el índice de fila de celda especificado.|
| [check_column(column_index)](/cells/es/python-net/aspose.cells/cells/check_column/#int) | Obtiene el elemento [Column](/cells/es/python-net/aspose.cells/column) o nulo en el índice de columna especificado.|
| [is_row_hidden(row_index)](/cells/es/python-net/aspose.cells/cells/is_row_hidden/#int) | Comprueba si una fila en el índice dado está oculta.|
| [is_column_hidden(column_index)](/cells/es/python-net/aspose.cells/cells/is_column_hidden/#int) | Comprueba si una columna en el índice dado está oculta.|
| [add_range(range_object)](/cells/es/python-net/aspose.cells/cells/add_range/#Range) | Agrega una referencia de objeto de rango a las celdas|
| [clear()](/cells/es/python-net/aspose.cells/cells/clear/#) | Borra todos los objetos de celda y fila.|
| [import_data(table, first_row, first_column, options)](/cells/es/python-net/aspose.cells/cells/import_data/#ICellsDataTable-int-int-ImportTableOptions) | Importar datos de la tabla de datos personalizados.|
| [import_array_list(array_list, first_row, first_column, is_vertical)](/cells/es/python-net/aspose.cells/cells/import_array_list/#list-int-int-bool) | Importa una lista de matriz de datos en una hoja de cálculo.|
| [import_formula_array(string_array, first_row, first_column, is_vertical)](/cells/es/python-net/aspose.cells/cells/import_formula_array/#list-int-int-bool) | Importa una matriz de fórmulas en una hoja de cálculo.|
| [text_to_columns(row, column, total_rows, options)](/cells/es/python-net/aspose.cells/cells/text_to_columns/#int-int-int-TxtLoadOptions) | Divide el texto de la columna en columnas.|
| [un_merge(first_row, first_column, total_rows, total_columns)](/cells/es/python-net/aspose.cells/cells/un_merge/#int-int-int-int) | Separa un rango específico de celdas combinadas.|
| [clear_merged_cells()](/cells/es/python-net/aspose.cells/cells/clear_merged_cells/#) | Borra todos los rangos combinados.|
| [hide_row(row)](/cells/es/python-net/aspose.cells/cells/hide_row/#int) | Oculta una fila.|
| [unhide_row(row, height)](/cells/es/python-net/aspose.cells/cells/unhide_row/#int-float) | Muestra una fila.|
| [hide_rows(row, total_rows)](/cells/es/python-net/aspose.cells/cells/hide_rows/#int-int) | Oculta varias filas.|
| [unhide_rows(row, total_rows, height)](/cells/es/python-net/aspose.cells/cells/unhide_rows/#int-int-float) | Muestra las filas ocultas.|
| [set_row_height_pixel(row, pixels)](/cells/es/python-net/aspose.cells/cells/set_row_height_pixel/#int-int) | Establece la altura de fila en unidades de píxeles.|
| [set_row_height_inch(row, inches)](/cells/es/python-net/aspose.cells/cells/set_row_height_inch/#int-float) | Establece la altura de la fila en unidades de pulgadas.|
| [set_row_height(row, height)](/cells/es/python-net/aspose.cells/cells/set_row_height/#int-float) | Establece la altura de la fila especificada.|
| [get_row_original_height_point(row)](/cells/es/python-net/aspose.cells/cells/get_row_original_height_point/#int) | Obtiene la altura de la fila original en unidades de punto si la fila está oculta|
| [hide_column(column)](/cells/es/python-net/aspose.cells/cells/hide_column/#int) | Oculta una columna.|
| [unhide_column(column, width)](/cells/es/python-net/aspose.cells/cells/unhide_column/#int-float) | Muestra una columna|
| [hide_columns(column, total_columns)](/cells/es/python-net/aspose.cells/cells/hide_columns/#int-int) | Ocultar varias columnas.|
| [unhide_columns(column, total_columns, width)](/cells/es/python-net/aspose.cells/cells/unhide_columns/#int-int-float) |Mostrar varias columnas.|
| [get_row_height(row)](/cells/es/python-net/aspose.cells/cells/get_row_height/#int) | Obtiene el alto de una fila especificada.|
| [get_view_row_height(row)](/cells/es/python-net/aspose.cells/cells/get_view_row_height/#int) | Obtiene el alto de una fila especificada.|
| [get_row_height_pixel(row)](/cells/es/python-net/aspose.cells/cells/get_row_height_pixel/#int) | Obtiene el alto de una fila especificada en unidades de píxel.|
| [get_row_height_inch(row)](/cells/es/python-net/aspose.cells/cells/get_row_height_inch/#int) | Obtiene el alto de una fila especificada en unidades de pulgadas.|
| [get_view_row_height_inch(row)](/cells/es/python-net/aspose.cells/cells/get_view_row_height_inch/#int) | Obtiene el alto de una fila especificada en unidades de pulgadas.|
| [set_column_width_pixel(column, pixels)](/cells/es/python-net/aspose.cells/cells/set_column_width_pixel/#int-int) | Establece el ancho de columna en unidades de píxeles en la vista normal.|
| [set_column_width_inch(column, inches)](/cells/es/python-net/aspose.cells/cells/set_column_width_inch/#int-float) | Establece el ancho de columna en unidades de pulgadas en la vista normal.|
| [set_column_width(column, width)](/cells/es/python-net/aspose.cells/cells/set_column_width/#int-float) | Establece el ancho de la columna especificada en la vista normal.|
| [get_column_width_pixel(column)](/cells/es/python-net/aspose.cells/cells/get_column_width_pixel/#int) | Obtiene el ancho de la columna especificada en vista normal, en unidades de píxel.|
| [get_column_width_inch(column)](/cells/es/python-net/aspose.cells/cells/get_column_width_inch/#int) | Obtiene el ancho de la columna especificada en vista normal, en unidades de pulgadas.|
| [get_column_width(column)](/cells/es/python-net/aspose.cells/cells/get_column_width/#int) | Obtiene el ancho de la columna especificada en la vista normal|
| [get_view_column_width_pixel(column)](/cells/es/python-net/aspose.cells/cells/get_view_column_width_pixel/#int) | Obtenga el ancho en diferentes tipos de vista.|
| [set_view_column_width_pixel(column, pixels)](/cells/es/python-net/aspose.cells/cells/set_view_column_width_pixel/#int-int) | Establece el ancho de la columna en una vista diferente.|
| [get_last_data_row(column)](/cells/es/python-net/aspose.cells/cells/get_last_data_row/#int) | Obtiene el índice de la última fila de la celda que contiene datos en la columna especificada.|
| [apply_column_style(column, style, flag)](/cells/es/python-net/aspose.cells/cells/apply_column_style/#int-Style-StyleFlag) | Aplica formatos para una columna completa.|
| [apply_row_style(row, style, flag)](/cells/es/python-net/aspose.cells/cells/apply_row_style/#int-Style-StyleFlag) | Aplica formatos para una fila completa.|
| [apply_style(style, flag)](/cells/es/python-net/aspose.cells/cells/apply_style/#Style-StyleFlag) | Aplica formatos para una hoja de cálculo completa.|
| [copy_column(source_cells, source_column_index, destination_column_index)](/cells/es/python-net/aspose.cells/cells/copy_column/#Cells-int-int) | Copia datos y formatos de una columna completa.|
| [copy_row(source_cells, source_row_index, destination_row_index)](/cells/es/python-net/aspose.cells/cells/copy_row/#Cells-int-int) | Copia datos y formatos de una fila completa.|
| [get_grouped_row_outline_level(row_index)](/cells/es/python-net/aspose.cells/cells/get_grouped_row_outline_level/#int) |Obtiene el nivel de esquema (basado en cero) de la fila.|
| [get_grouped_column_outline_level(column_index)](/cells/es/python-net/aspose.cells/cells/get_grouped_column_outline_level/#int) | Obtiene el nivel de esquema (basado en cero) de la columna.|
| [get_max_grouped_column_outline_level()](/cells/es/python-net/aspose.cells/cells/get_max_grouped_column_outline_level/#) | Obtiene el nivel máximo de esquema de columna agrupada (basado en cero).|
| [get_max_grouped_row_outline_level()](/cells/es/python-net/aspose.cells/cells/get_max_grouped_row_outline_level/#) | Obtiene el nivel máximo de esquema de filas agrupadas (basado en cero).|
| [show_group_detail(is_vertical, index)](/cells/es/python-net/aspose.cells/cells/show_group_detail/#bool-int) | Expande las filas/columnas agrupadas.|
| [hide_group_detail(is_vertical, index)](/cells/es/python-net/aspose.cells/cells/hide_group_detail/#bool-int) | Contrae las filas/columnas agrupadas.|
| [ungroup_columns(first_index, last_index)](/cells/es/python-net/aspose.cells/cells/ungroup_columns/#int-int) | Desagrupa columnas.|
| [delete_columns(column_index, total_columns, update_reference)](/cells/es/python-net/aspose.cells/cells/delete_columns/#int-int-bool) | Elimina varias columnas.|
| [is_deleting_range_enabled(start_row, start_column, total_rows, total_columns)](/cells/es/python-net/aspose.cells/cells/is_deleting_range_enabled/#int-int-int-int) | Compruebe si se puede eliminar el intervalo.|
| [delete_row(row_index)](/cells/es/python-net/aspose.cells/cells/delete_row/#int) | Elimina una fila.|
| [is_blank_column(column_index)](/cells/es/python-net/aspose.cells/cells/is_blank_column/#int) | Comprueba si la columna dada está en blanco (no contiene ningún dato).|
| [insert_row(row_index)](/cells/es/python-net/aspose.cells/cells/insert_row/#int) | Inserta una nueva fila en la hoja de trabajo.|
| [link_to_xml_map(map_name, row, column, path)](/cells/es/python-net/aspose.cells/cells/link_to_xml_map/#str-int-int-str) | Enlace a un mapa xml.|
| [find_formula(formula, previous_cell)](/cells/es/python-net/aspose.cells/cells/find_formula/#str-Cell) | Encuentra la celda con la cadena de entrada.|
| [find_formula_contains(formula, previous_cell)](/cells/es/python-net/aspose.cells/cells/find_formula_contains/#str-Cell) | Encuentra la celda con la fórmula que contiene la cadena de entrada.|
| [move_range(source_area, dest_row, dest_column)](/cells/es/python-net/aspose.cells/cells/move_range/#CellArea-int-int) | Mueve el rango.|
| [insert_cut_cells(cut_range, row, column, shift_type)](/cells/es/python-net/aspose.cells/cells/insert_cut_cells/#Range-int-int-ShiftType) | Rango de corte de inserción.|
| [delete_range(start_row, start_column, end_row, end_column, shift_type)](/cells/es/python-net/aspose.cells/cells/delete_range/#int-int-int-int-ShiftType) | Elimina un rango de celdas y desplaza celdas según la opción de desplazamiento.|
| [retrieve_subtotal_setting(ca)](/cells/es/python-net/aspose.cells/cells/retrieve_subtotal_setting/#CellArea) | Recupera la configuración de subtotales del rango.|
| [remove_formulas()](/cells/es/python-net/aspose.cells/cells/remove_formulas/#) | Elimina todas las fórmulas y las reemplaza con el valor de la fórmula.|
| [convert_string_to_numeric_value()](/cells/es/python-net/aspose.cells/cells/convert_string_to_numeric_value/#) |Convierte datos de cadena en celdas a valor numérico si es posible.|
| [get_dependents(is_all, row, column)](/cells/es/python-net/aspose.cells/cells/get_dependents/#bool-int-int) | Obtenga todas las celdas que se refieren a la celda específica.|
| [get_dependents_in_calculation(row, column, recursive)](/cells/es/python-net/aspose.cells/cells/get_dependents_in_calculation/#int-int-bool) | Obtiene todas las celdas cuyo resultado calculado depende de una celda específica.|
| [get_cell_style(row, column)](/cells/es/python-net/aspose.cells/cells/get_cell_style/#int-int) | Obtener el estilo de la celda dada.|



###  Ver también
* módulo [aspose.cells](..)
* clase [Cell](/cells/es/python-net/aspose.cells/cell)
* clase [Column](/cells/es/python-net/aspose.cells/column)
* clase [Range](/cells/es/python-net/aspose.cells/range)
* clase [Row](/cells/es/python-net/aspose.cells/row)
