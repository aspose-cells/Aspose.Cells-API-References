---
title: classe ShapeCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 530
url: /it/python-net/aspose.cells.drawing/shapecollection/
is_root: false
---
##  classe ShapeCollection
Rappresenta tutta la forma in un foglio di lavoro/grafico.



Il tipo ShapeCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells.drawing/shapecollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add_shape_in_chart(type, placement, left, top, right, bottom, image_data)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int-bytes) | Aggiungi una forma al grafico. Tutte le unità sono 1/4000 dell'area del grafico.|
| [add_shape_in_chart(type, placement, left, top, right, bottom)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int) | Aggiungi una forma al grafico. Tutte le unità sono 1/4000 dell'area del grafico.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float) | Aggiungi una forma al grafico. Tutte le unità sono la scala percentuale dell'area del grafico.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom, image_data)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float-bytes) | Aggiungi una forma al grafico. Tutte le unità sono 1/4000 dell'area del grafico.|
| [add_picture(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-int-int-io.RawIOBase) | Aggiunge un'immagine alla raccolta.|
| [add_picture(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-io.RawIOBase-int-int) | Aggiunge un'immagine alla raccolta.|
| [copy_to(array)](/cells/it/python-net/aspose.cells.drawing/shapecollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells.drawing/shapecollection/copy_to/#int-list-int-int) |Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [add_copy(source_shape, upper_left_row, top, upper_left_column, left)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_copy/#Shape-int-int-int-int) | Aggiunge e copia una forma nel foglio di lavoro.|
| [add_check_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_check_box/#int-int-int-int-int-int) | Aggiunge una casella di controllo al foglio di lavoro.|
| [add_text_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_text_box/#int-int-int-int-int-int) | Aggiunge una casella di testo al foglio di lavoro.|
| [add_spinner(upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_spinner/#int-int-int-int-int-int) | Aggiunge uno Spinner al foglio di lavoro.|
| [add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/#int-int-int-int-int-int) | Aggiunge una barra di scorrimento al foglio di lavoro.|
| [add_radio_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_radio_button/#int-int-int-int-int-int) | Aggiunge un RadioButton al foglio di lavoro.|
| [add_list_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_list_box/#int-int-int-int-int-int) | Aggiunge un ListBox al foglio di lavoro.|
| [add_combo_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_combo_box/#int-int-int-int-int-int) | Aggiunge un ComboBox al foglio di lavoro.|
| [add_group_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_group_box/#int-int-int-int-int-int) |Aggiunge un GroupBox al foglio di lavoro.|
| [add_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_button/#int-int-int-int-int-int) | Aggiunge un pulsante al foglio di lavoro.|
| [add_label(upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_label/#int-int-int-int-int-int) | Aggiunge un'etichetta al foglio di lavoro.|
| [add_label_in_chart(top, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_label_in_chart/#int-int-int-int) | Aggiunge un'etichetta al grafico.|
| [add_text_box_in_chart(top, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_text_box_in_chart/#int-int-int-int) | Aggiunge una casella di testo al grafico.|
| [add_text_effect_in_chart(effect, text, font_name, size, font_bold, font_italic, top, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_text_effect_in_chart/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int) | Inserisce un oggetto WordArt nel grafico|
| [add_text_effect(effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_text_effect/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int-int-int) | Inserisce un oggetto WordArt.|
| [add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_word_art/#PresetWordArtStyle-str-int-int-int-int-int-int) | Aggiunge WordArt preimpostato da Excel 2007.s|
| [add_rectangle(upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_rectangle/#int-int-int-int-int-int) | Aggiunge un oggetto RectangleShape al foglio di lavoro.|
| [add_oval(upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_oval/#int-int-int-int-int-int) | Aggiunge un ovale al foglio di lavoro.|
| [add_line(upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_line/#int-int-int-int-int-int) | Aggiunge un oggetto LineShape al foglio di lavoro.|
| [add_free_floating_shape(type, top, left, height, width, image_data, is_original_size)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/#MsoDrawingType-int-int-int-int-bytes-bool) | Aggiunge una forma fluttuante libera al foglio di lavoro. Si applica solo alla forma linea/immagine.|
| [add_arc(upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_arc/#int-int-int-int-int-int) | Aggiunge un ArcShape al foglio di lavoro.|
| [add_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_shape/#MsoDrawingType-int-int-int-int-int-int) | Aggiunge una forma al foglio di lavoro.|
| [add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/#AutoShapeType-int-int-int-int-int-int) | Aggiunge una forma al foglio di lavoro.|
| [add_auto_shape_in_chart(type, top, left, height, width)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_auto_shape_in_chart/#AutoShapeType-int-int-int-int) | Aggiunge una forma al grafico.|
| [add_active_x_control(type, top_row, top, left_column, left, width, height)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int) | Crea un controllo Activex.|
| [add_svg(upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_svg/#int-int-int-int-int-int-bytes-bytes) | Aggiunge un'immagine svg.|
| [add_icons(upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_icons/#int-int-int-int-int-int-bytes-bytes) | Aggiunge un'immagine svg.|
| [add_linked_picture(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_linked_picture/#int-int-int-int-str) | Aggiungi un'immagine collegata.|
| [add_ole_object_with_linked_image(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_ole_object_with_linked_image/#int-int-int-int-str) | Aggiungi un'immagine collegata.|
| [add_picture_in_chart(top, left, stream, width_scale, height_scale)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_picture_in_chart/#int-int-io.RawIOBase-int-int) | Aggiunge un'immagine al grafico.|
| [add_ole_object(upper_left_row, top, upper_left_column, left, height, width, image_data)](/cells/it/python-net/aspose.cells.drawing/shapecollection/add_ole_object/#int-int-int-int-int-int-bytes) | Aggiunge un OleObject.|
| [copy_comments_in_range(shapes, ca, dest_row, dest_column)](/cells/it/python-net/aspose.cells.drawing/shapecollection/copy_comments_in_range/#ShapeCollection-CellArea-int-int) | Copia tutti i commenti nell'intervallo.|
| [copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained)](/cells/it/python-net/aspose.cells.drawing/shapecollection/copy_in_range/#ShapeCollection-CellArea-int-int-bool) | Copia le forme nell'intervallo nell'intervallo di destinazione.|
| [delete_in_range(ca)](/cells/it/python-net/aspose.cells.drawing/shapecollection/delete_in_range/#CellArea) | Elimina le forme nell'intervallo. Le forme dei commenti non verranno eliminate.|
| [delete_shape(shape)](/cells/it/python-net/aspose.cells.drawing/shapecollection/delete_shape/#Shape) |Elimina una forma. Se la forma è nel gruppo o è una forma di commento, non verrà eliminata.|
| [group(group_items)](/cells/it/python-net/aspose.cells.drawing/shapecollection/group/#list) | Raggruppa le forme.|
| [ungroup(group)](/cells/it/python-net/aspose.cells.drawing/shapecollection/ungroup/#GroupShape) | Separa gli elementi della forma.|
| [update_selected_value()](/cells/it/python-net/aspose.cells.drawing/shapecollection/update_selected_value/#) | Aggiorna il valore selezionato in base al valore della cella collegata delle forme.|
| [binary_search(item)](/cells/it/python-net/aspose.cells.drawing/shapecollection/binary_search/#Shape) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempio

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

###  Guarda anche
* modulo [aspose.cells.drawing](..)
