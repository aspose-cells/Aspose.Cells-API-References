---
title: ShapeCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 530
url: /es/python-net/aspose.cells.drawing/shapecollection/
is_root: false
---
##  ShapeCollection clase
Representa todas las formas en una hoja de cálculo/gráfico.



El tipo ShapeCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells.drawing/shapecollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add_shape_in_chart(type, placement, left, top, right, bottom, image_data)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int-bytes) | Agregue una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico.|
| [add_shape_in_chart(type, placement, left, top, right, bottom)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int) | Agregue una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float) | Agrega una forma al gráfico. Todas las unidades son una escala porcentual del área del gráfico.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom, image_data)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float-bytes) | Agregue una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico.|
| [add_picture(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-int-int-io.RawIOBase) | Agrega una imagen a la colección.|
| [add_picture(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-io.RawIOBase-int-int) | Agrega una imagen a la colección.|
| [copy_to(array)](/cells/es/python-net/aspose.cells.drawing/shapecollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells.drawing/shapecollection/copy_to/#int-list-int-int) |Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [add_copy(source_shape, upper_left_row, top, upper_left_column, left)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_copy/#Shape-int-int-int-int) | Agrega y copia una forma a la hoja de trabajo.|
| [add_check_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_check_box/#int-int-int-int-int-int) | Agrega una casilla de verificación a la hoja de cálculo.|
| [add_text_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_text_box/#int-int-int-int-int-int) | Agrega un cuadro de texto a la hoja de cálculo.|
| [add_spinner(upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_spinner/#int-int-int-int-int-int) | Agrega un Spinner a la hoja de trabajo.|
| [add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/#int-int-int-int-int-int) | Agrega una barra de desplazamiento a la hoja de cálculo.|
| [add_radio_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_radio_button/#int-int-int-int-int-int) | Agrega un RadioButton a la hoja de cálculo.|
| [add_list_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_list_box/#int-int-int-int-int-int) | Agrega un ListBox a la hoja de trabajo.|
| [add_combo_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_combo_box/#int-int-int-int-int-int) | Agrega un ComboBox a la hoja de trabajo.|
| [add_group_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_group_box/#int-int-int-int-int-int) |Agrega un GroupBox a la hoja de cálculo.|
| [add_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_button/#int-int-int-int-int-int) | Agrega un botón a la hoja de trabajo.|
| [add_label(upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_label/#int-int-int-int-int-int) | Agrega una etiqueta a la hoja de trabajo.|
| [add_label_in_chart(top, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_label_in_chart/#int-int-int-int) | Agrega una etiqueta al gráfico.|
| [add_text_box_in_chart(top, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_text_box_in_chart/#int-int-int-int) | Agrega un cuadro de texto al gráfico.|
| [add_text_effect_in_chart(effect, text, font_name, size, font_bold, font_italic, top, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_text_effect_in_chart/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int) | Inserta un objeto de WordArt en el gráfico.|
| [add_text_effect(effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_text_effect/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int-int-int) | Inserta un objeto de WordArt.|
| [add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_word_art/#PresetWordArtStyle-str-int-int-int-int-int-int) | Agrega WordArt predeterminado desde Excel 2007.s|
| [add_rectangle(upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_rectangle/#int-int-int-int-int-int) | Agrega un RectangleShape a la hoja de cálculo.|
| [add_oval(upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_oval/#int-int-int-int-int-int) | Agrega un óvalo a la hoja de cálculo.|
| [add_line(upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_line/#int-int-int-int-int-int) | Agrega un LineShape a la hoja de cálculo.|
| [add_free_floating_shape(type, top, left, height, width, image_data, is_original_size)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/#MsoDrawingType-int-int-int-int-bytes-bool) | Agrega una forma flotante libre a la hoja de cálculo. Solo se aplica a la forma de línea/imagen.|
| [add_arc(upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_arc/#int-int-int-int-int-int) | Agrega un ArcShape a la hoja de trabajo.|
| [add_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_shape/#MsoDrawingType-int-int-int-int-int-int) | Agrega una forma a la hoja de cálculo.|
| [add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/#AutoShapeType-int-int-int-int-int-int) | Agrega una autoforma a la hoja de trabajo.|
| [add_auto_shape_in_chart(type, top, left, height, width)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_auto_shape_in_chart/#AutoShapeType-int-int-int-int) | Agrega una autoforma al gráfico.|
| [add_active_x_control(type, top_row, top, left_column, left, width, height)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int) | Crea un Control Activex.|
| [add_svg(upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_svg/#int-int-int-int-int-int-bytes-bytes) | Agrega imagen svg.|
| [add_icons(upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_icons/#int-int-int-int-int-int-bytes-bytes) | Agrega imagen svg.|
| [add_linked_picture(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_linked_picture/#int-int-int-int-str) | Agrega una imagen vinculada.|
| [add_ole_object_with_linked_image(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_ole_object_with_linked_image/#int-int-int-int-str) | Agrega una imagen vinculada.|
| [add_picture_in_chart(top, left, stream, width_scale, height_scale)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_picture_in_chart/#int-int-io.RawIOBase-int-int) | Agrega una imagen al gráfico.|
| [add_ole_object(upper_left_row, top, upper_left_column, left, height, width, image_data)](/cells/es/python-net/aspose.cells.drawing/shapecollection/add_ole_object/#int-int-int-int-int-int-bytes) | Agrega un OleObject.|
| [copy_comments_in_range(shapes, ca, dest_row, dest_column)](/cells/es/python-net/aspose.cells.drawing/shapecollection/copy_comments_in_range/#ShapeCollection-CellArea-int-int) | Copie todos los comentarios en el rango.|
| [copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained)](/cells/es/python-net/aspose.cells.drawing/shapecollection/copy_in_range/#ShapeCollection-CellArea-int-int-bool) | Copie formas en el rango al rango de destino.|
| [delete_in_range(ca)](/cells/es/python-net/aspose.cells.drawing/shapecollection/delete_in_range/#CellArea) | Eliminar formas en el rango. Las formas de comentarios no se eliminarán.|
| [delete_shape(shape)](/cells/es/python-net/aspose.cells.drawing/shapecollection/delete_shape/#Shape) |Eliminar una forma. Si la forma está en el grupo o es una forma de comentario, no se eliminará.|
| [group(group_items)](/cells/es/python-net/aspose.cells.drawing/shapecollection/group/#list) | Agrupa las formas.|
| [ungroup(group)](/cells/es/python-net/aspose.cells.drawing/shapecollection/ungroup/#GroupShape) | Desagrupa los elementos de forma.|
| [update_selected_value()](/cells/es/python-net/aspose.cells.drawing/shapecollection/update_selected_value/#) | Actualice el valor seleccionado por el valor de la celda vinculada de las formas.|
| [binary_search(item)](/cells/es/python-net/aspose.cells.drawing/shapecollection/binary_search/#Shape) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplo

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# get ShapeCollection
shapes = workbook.worksheets[0].shapes
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

###  Ver también
* módulo [aspose.cells.drawing](..)
