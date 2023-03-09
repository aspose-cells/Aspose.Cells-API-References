---
title: ShapeCollection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 530
url: /sv/python-net/aspose.cells.drawing/shapecollection/
is_root: false
---
##  ShapeCollection klass
Representerar all form i ett kalkylblad/diagram.



Typen ShapeCollection avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [capacity](/cells/sv/python-net/aspose.cells.drawing/shapecollection/capacity) | Hämtar eller ställer in antalet element som arraylistan kan innehålla.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [add_shape_in_chart(type, placement, left, top, right, bottom, image_data)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int-bytes) | Lägg till en form i diagrammet. Alla enheter är 1/4000 av kartytan.|
| [add_shape_in_chart(type, placement, left, top, right, bottom)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int) | Lägg till en form i diagrammet. Alla enheter är 1/4000 av kartytan.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float) | Lägg till en form i diagrammet. Alla enheter är procentuell skala av diagramområdet.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom, image_data)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float-bytes) | Lägg till en form i diagrammet. Alla enheter är 1/4000 av kartytan.|
| [add_picture(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-int-int-io.RawIOBase) | Lägger till en bild i samlingen.|
| [add_picture(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-io.RawIOBase-int-int) | Lägger till en bild i samlingen.|
| [copy_to(array)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/copy_to/#list) | Kopierar hela arraylistan till en kompatibel endimensionell arraylista, med början i början av målarraylistan.|
| [copy_to(index, array, array_index, count)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/copy_to/#int-list-int-int) | Kopierar ett intervall av element från arraylistan till en kompatibel endimensionell arraylista, med början vid det angivna indexet för målarraylistan.|
| [index_of(item, index)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som sträcker sig från det angivna indexet till det sista elementet.|
| [index_of(item, index, count)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som börjar vid det angivna indexet och innehåller det angivna antalet element.|
| [last_index_of(item)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom hela arraylistan.|
| [last_index_of(item, index)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int) |Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som sträcker sig från det första elementet till det angivna indexet.|
| [last_index_of(item, index, count)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som innehåller det angivna antalet element och slutar vid det angivna indexet.|
| [add_copy(source_shape, upper_left_row, top, upper_left_column, left)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_copy/#Shape-int-int-int-int) | Lägger till och kopierar en form till kalkylbladet.|
| [add_check_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_check_box/#int-int-int-int-int-int) | Lägger till en kryssruta i kalkylbladet.|
| [add_text_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_text_box/#int-int-int-int-int-int) |Lägger till en textruta i kalkylbladet.|
| [add_spinner(upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_spinner/#int-int-int-int-int-int) | Lägger till en Spinner i arbetsbladet.|
| [add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/#int-int-int-int-int-int) | Lägger till en rullningslist i arbetsbladet.|
| [add_radio_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_radio_button/#int-int-int-int-int-int) | Lägger till en RadioButton i arbetsbladet.|
| [add_list_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_list_box/#int-int-int-int-int-int) | Lägger till en ListBox i kalkylbladet.|
| [add_combo_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_combo_box/#int-int-int-int-int-int) | Lägger till en ComboBox i kalkylbladet.|
| [add_group_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_group_box/#int-int-int-int-int-int) | Lägger till en GroupBox i kalkylbladet.|
| [add_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_button/#int-int-int-int-int-int) | Lägger till en knapp i arbetsbladet.|
| [add_label(upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_label/#int-int-int-int-int-int) | Lägger till en etikett i arbetsbladet.|
| [add_label_in_chart(top, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_label_in_chart/#int-int-int-int) | Lägger till en etikett i diagrammet.|
| [add_text_box_in_chart(top, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_text_box_in_chart/#int-int-int-int) | Lägger till en textruta i diagrammet.|
| [add_text_effect_in_chart(effect, text, font_name, size, font_bold, font_italic, top, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_text_effect_in_chart/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int) | Infogar ett WordArt-objekt i diagrammet|
| [add_text_effect(effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_text_effect/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int-int-int) | Infogar ett WordArt-objekt.|
| [add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_word_art/#PresetWordArtStyle-str-int-int-int-int-int-int) | Lägger till förinställd WordArt sedan Excel 2007.s|
| [add_rectangle(upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_rectangle/#int-int-int-int-int-int) | Lägger till en RectangleShape till kalkylbladet.|
| [add_oval(upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_oval/#int-int-int-int-int-int) | Lägger till en oval i arbetsbladet.|
| [add_line(upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_line/#int-int-int-int-int-int) | Lägger till en LineShape i kalkylbladet.|
| [add_free_floating_shape(type, top, left, height, width, image_data, is_original_size)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/#MsoDrawingType-int-int-int-int-bytes-bool) | Lägger till en fri flytande form till kalkylbladet. Gäller endast linje-/bildform.|
| [add_arc(upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_arc/#int-int-int-int-int-int) | Lägger till en ArcShape i kalkylbladet.|
| [add_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_shape/#MsoDrawingType-int-int-int-int-int-int) | Lägger till en form i kalkylbladet.|
| [add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/#AutoShapeType-int-int-int-int-int-int) |Lägger till en AutoShape i kalkylbladet.|
| [add_auto_shape_in_chart(type, top, left, height, width)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_auto_shape_in_chart/#AutoShapeType-int-int-int-int) | Lägger till en AutoShape i diagrammet.|
| [add_active_x_control(type, top_row, top, left_column, left, width, height)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int) | Skapar en Activex-kontroll.|
| [add_svg(upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_svg/#int-int-int-int-int-int-bytes-bytes) | Lägger till svg-bild.|
| [add_icons(upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_icons/#int-int-int-int-int-int-bytes-bytes) | Lägger till svg-bild.|
| [add_linked_picture(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_linked_picture/#int-int-int-int-str) | Lägg till en länkad bild.|
| [add_ole_object_with_linked_image(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_ole_object_with_linked_image/#int-int-int-int-str) | Lägg till en länkad bild.|
| [add_picture_in_chart(top, left, stream, width_scale, height_scale)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_picture_in_chart/#int-int-io.RawIOBase-int-int) | Lägger till en bild i diagrammet.|
| [add_ole_object(upper_left_row, top, upper_left_column, left, height, width, image_data)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/add_ole_object/#int-int-int-int-int-int-bytes) | Lägger till ett OleObject.|
| [copy_comments_in_range(shapes, ca, dest_row, dest_column)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/copy_comments_in_range/#ShapeCollection-CellArea-int-int) | Kopiera alla kommentarer i sortimentet.|
| [copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/copy_in_range/#ShapeCollection-CellArea-int-int-bool) | Kopiera former i intervallet till destinationsintervallet.|
| [delete_in_range(ca)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/delete_in_range/#CellArea) | Ta bort former i intervallet. Kommentarsformer kommer inte att tas bort.|
| [delete_shape(shape)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/delete_shape/#Shape) | Ta bort en form. Om formen finns i gruppen eller är en kommentarsform kommer den inte att tas bort.|
| [group(group_items)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/group/#list) | Gruppera formerna.|
| [ungroup(group)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/ungroup/#GroupShape) | Delar upp formobjekten.|
| [update_selected_value()](/cells/sv/python-net/aspose.cells.drawing/shapecollection/update_selected_value/#) | Uppdatera det valda värdet med värdet för den länkade cellen i formerna.|
| [binary_search(item)](/cells/sv/python-net/aspose.cells.drawing/shapecollection/binary_search/#Shape) | Söker i hela den sorterade arraylistan efter ett element med hjälp av standardjämföraren och returnerar elementets nollbaserade index.|



###  Exempel

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

###  Se även
* modul [aspose.cells.drawing](..)
