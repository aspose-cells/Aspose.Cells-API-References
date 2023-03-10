---
title: ShapeCollection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 530
url: /de/python-net/aspose.cells.drawing/shapecollection/
is_root: false
---
##  ShapeCollection Klasse
Stellt alle Formen in einem Arbeitsblatt/Diagramm dar.



Der Typ ShapeCollection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [capacity](/cells/de/python-net/aspose.cells.drawing/shapecollection/capacity) | Ruft die Anzahl der Elemente ab, die die Arrayliste enthalten kann, oder legt diese fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [add_shape_in_chart(type, placement, left, top, right, bottom, image_data)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int-bytes) | Fügen Sie dem Diagramm eine Form hinzu. Alle Einheiten sind 1/4000 des Diagrammbereichs.|
| [add_shape_in_chart(type, placement, left, top, right, bottom)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int) | Fügen Sie dem Diagramm eine Form hinzu. Alle Einheiten sind 1/4000 des Diagrammbereichs.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float) | Fügen Sie dem Diagramm eine Form hinzu. Alle Einheiten sind Prozentskalen des Diagrammbereichs.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom, image_data)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float-bytes) | Fügen Sie dem Diagramm eine Form hinzu. Alle Einheiten sind 1/4000 des Diagrammbereichs.|
| [add_picture(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-int-int-io.RawIOBase) | Fügt der Sammlung ein Bild hinzu.|
| [add_picture(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-io.RawIOBase-int-int) | Fügt der Sammlung ein Bild hinzu.|
| [copy_to(array)](/cells/de/python-net/aspose.cells.drawing/shapecollection/copy_to/#list) | Kopiert die gesamte Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am Anfang der Ziel-Array-Liste.|
| [copy_to(index, array, array_index, count)](/cells/de/python-net/aspose.cells.drawing/shapecollection/copy_to/#int-list-int-int) |Kopiert eine Reihe von Elementen aus der Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am angegebenen Index der Ziel-Array-Liste.|
| [index_of(item, index)](/cells/de/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom angegebenen Index bis zum letzten Element erstreckt.|
| [index_of(item, index, count)](/cells/de/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der am angegebenen Index beginnt und die angegebene Anzahl von Elementen enthält.|
| [last_index_of(item)](/cells/de/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens in der gesamten Array-Liste zurück.|
| [last_index_of(item, index)](/cells/de/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom ersten Element bis zum angegebenen Index erstreckt.|
| [last_index_of(item, index, count)](/cells/de/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int-int) |Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der die angegebene Anzahl von Elementen enthält und am angegebenen Index endet.|
| [add_copy(source_shape, upper_left_row, top, upper_left_column, left)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_copy/#Shape-int-int-int-int) | Fügt eine Form zum Arbeitsblatt hinzu und kopiert sie.|
| [add_check_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_check_box/#int-int-int-int-int-int) | Fügt dem Arbeitsblatt ein Kontrollkästchen hinzu.|
| [add_text_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_text_box/#int-int-int-int-int-int) | Fügt dem Arbeitsblatt ein Textfeld hinzu.|
| [add_spinner(upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_spinner/#int-int-int-int-int-int) | Fügt dem Arbeitsblatt ein Kreisel hinzu.|
| [add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/#int-int-int-int-int-int) | Fügt dem Arbeitsblatt eine ScrollBar hinzu.|
| [add_radio_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_radio_button/#int-int-int-int-int-int) | Fügt dem Arbeitsblatt einen RadioButton hinzu.|
| [add_list_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_list_box/#int-int-int-int-int-int) | Fügt dem Arbeitsblatt eine ListBox hinzu.|
| [add_combo_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_combo_box/#int-int-int-int-int-int) | Fügt dem Arbeitsblatt eine ComboBox hinzu.|
| [add_group_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_group_box/#int-int-int-int-int-int) |Fügt dem Arbeitsblatt eine GroupBox hinzu.|
| [add_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_button/#int-int-int-int-int-int) | Fügt dem Arbeitsblatt eine Schaltfläche hinzu.|
| [add_label(upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_label/#int-int-int-int-int-int) | Fügt dem Arbeitsblatt eine Beschriftung hinzu.|
| [add_label_in_chart(top, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_label_in_chart/#int-int-int-int) | Fügt dem Diagramm eine Beschriftung hinzu.|
| [add_text_box_in_chart(top, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_text_box_in_chart/#int-int-int-int) | Fügt dem Diagramm ein Textfeld hinzu.|
| [add_text_effect_in_chart(effect, text, font_name, size, font_bold, font_italic, top, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_text_effect_in_chart/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int) | Fügt ein WordArt-Objekt in das Diagramm ein|
| [add_text_effect(effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_text_effect/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int-int-int) | Fügt ein WordArt-Objekt ein.|
| [add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_word_art/#PresetWordArtStyle-str-int-int-int-int-int-int) | Fügt voreingestelltes WordArt seit Excel 2007.s hinzu|
| [add_rectangle(upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_rectangle/#int-int-int-int-int-int) | Fügt dem Arbeitsblatt ein RectangleShape hinzu.|
| [add_oval(upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_oval/#int-int-int-int-int-int) | Fügt dem Arbeitsblatt ein Oval hinzu.|
| [add_line(upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_line/#int-int-int-int-int-int) | Fügt dem Arbeitsblatt eine Linienform hinzu.|
| [add_free_floating_shape(type, top, left, height, width, image_data, is_original_size)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/#MsoDrawingType-int-int-int-int-bytes-bool) | Fügt dem Arbeitsblatt eine freischwebende Form hinzu. Gilt nur für Linien-/Bildform.|
| [add_arc(upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_arc/#int-int-int-int-int-int) | Fügt dem Arbeitsblatt eine ArcShape hinzu.|
| [add_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_shape/#MsoDrawingType-int-int-int-int-int-int) | Fügt dem Arbeitsblatt eine Form hinzu.|
| [add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/#AutoShapeType-int-int-int-int-int-int) | Fügt dem Arbeitsblatt eine AutoForm hinzu.|
| [add_auto_shape_in_chart(type, top, left, height, width)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_auto_shape_in_chart/#AutoShapeType-int-int-int-int) | Fügt dem Diagramm eine AutoForm hinzu.|
| [add_active_x_control(type, top_row, top, left_column, left, width, height)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int) | Erstellt ein Activex-Steuerelement.|
| [add_svg(upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_svg/#int-int-int-int-int-int-bytes-bytes) | Fügt ein SVG-Bild hinzu.|
| [add_icons(upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_icons/#int-int-int-int-int-int-bytes-bytes) | Fügt ein SVG-Bild hinzu.|
| [add_linked_picture(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_linked_picture/#int-int-int-int-str) | Füge ein verlinktes Bild hinzu.|
| [add_ole_object_with_linked_image(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_ole_object_with_linked_image/#int-int-int-int-str) | Füge ein verlinktes Bild hinzu.|
| [add_picture_in_chart(top, left, stream, width_scale, height_scale)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_picture_in_chart/#int-int-io.RawIOBase-int-int) | Fügt dem Diagramm ein Bild hinzu.|
| [add_ole_object(upper_left_row, top, upper_left_column, left, height, width, image_data)](/cells/de/python-net/aspose.cells.drawing/shapecollection/add_ole_object/#int-int-int-int-int-int-bytes) | Fügt ein OleObject hinzu.|
| [copy_comments_in_range(shapes, ca, dest_row, dest_column)](/cells/de/python-net/aspose.cells.drawing/shapecollection/copy_comments_in_range/#ShapeCollection-CellArea-int-int) | Kopieren Sie alle Kommentare im Bereich.|
| [copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained)](/cells/de/python-net/aspose.cells.drawing/shapecollection/copy_in_range/#ShapeCollection-CellArea-int-int-bool) | Formen im Bereich in den Zielbereich kopieren.|
| [delete_in_range(ca)](/cells/de/python-net/aspose.cells.drawing/shapecollection/delete_in_range/#CellArea) | Formen im Bereich löschen.Kommentarformen werden nicht gelöscht.|
| [delete_shape(shape)](/cells/de/python-net/aspose.cells.drawing/shapecollection/delete_shape/#Shape) |Löschen Sie eine Form. Wenn sich die Form in der Gruppe befindet oder eine Kommentarform ist, wird sie nicht gelöscht.|
| [group(group_items)](/cells/de/python-net/aspose.cells.drawing/shapecollection/group/#list) | Gruppieren Sie die Formen.|
| [ungroup(group)](/cells/de/python-net/aspose.cells.drawing/shapecollection/ungroup/#GroupShape) | Hebt die Gruppierung der Formelemente auf.|
| [update_selected_value()](/cells/de/python-net/aspose.cells.drawing/shapecollection/update_selected_value/#) | Aktualisieren Sie den ausgewählten Wert um den Wert der verknüpften Zelle der Formen.|
| [binary_search(item)](/cells/de/python-net/aspose.cells.drawing/shapecollection/binary_search/#Shape) | Durchsucht die gesamte sortierte Array-Liste mithilfe des Standardvergleichs nach einem Element und gibt den nullbasierten Index des Elements zurück.|



###  Beispiel

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

###  Siehe auch
* Modul [aspose.cells.drawing](..)
