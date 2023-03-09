---
title: ShapeCollection sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 530
url: /tr/python-net/aspose.cells.drawing/shapecollection/
is_root: false
---
##  ShapeCollection sınıfı
Bir çalışma sayfasındaki/grafikteki tüm şekilleri temsil eder.



ShapeCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [capacity](/cells/tr/python-net/aspose.cells.drawing/shapecollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add_shape_in_chart(type, placement, left, top, right, bottom, image_data)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int-bytes) | Grafiğe bir şekil ekleyin. Tüm birimler grafik alanının 1/4000'idir.|
| [add_shape_in_chart(type, placement, left, top, right, bottom)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int) | Grafiğe bir şekil ekleyin. Tüm birimler grafik alanının 1/4000'idir.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float) | Grafiğe bir şekil ekleyin. Tüm birimler, grafik alanının yüzde ölçeğidir.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom, image_data)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float-bytes) | Grafiğe bir şekil ekleyin. Tüm birimler grafik alanının 1/4000'idir.|
| [add_picture(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-int-int-io.RawIOBase) | Koleksiyona bir resim ekler.|
| [add_picture(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-io.RawIOBase-int-int) | Koleksiyona bir resim ekler.|
| [copy_to(array)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/copy_to/#int-list-int-int) |Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int) | Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int-int) |Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [add_copy(source_shape, upper_left_row, top, upper_left_column, left)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_copy/#Shape-int-int-int-int) | Çalışma sayfasına bir şekil ekler ve kopyalar.|
| [add_check_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_check_box/#int-int-int-int-int-int) | Çalışma sayfasına bir onay kutusu ekler.|
| [add_text_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_text_box/#int-int-int-int-int-int) | Çalışma sayfasına bir metin kutusu ekler.|
| [add_spinner(upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_spinner/#int-int-int-int-int-int) | Çalışma sayfasına bir Döndürücü ekler.|
| [add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/#int-int-int-int-int-int) | Çalışma sayfasına bir ScrollBar ekler.|
| [add_radio_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_radio_button/#int-int-int-int-int-int) | Çalışma sayfasına bir RadioButton ekler.|
| [add_list_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_list_box/#int-int-int-int-int-int) | Çalışma sayfasına bir ListBox ekler.|
| [add_combo_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_combo_box/#int-int-int-int-int-int) | Çalışma sayfasına bir ComboBox ekler.|
| [add_group_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_group_box/#int-int-int-int-int-int) |Çalışma sayfasına bir GroupBox ekler.|
| [add_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_button/#int-int-int-int-int-int) | Çalışma sayfasına bir Düğme ekler.|
| [add_label(upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_label/#int-int-int-int-int-int) | Çalışma sayfasına bir Etiket ekler.|
| [add_label_in_chart(top, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_label_in_chart/#int-int-int-int) | Grafiğe bir etiket ekler.|
| [add_text_box_in_chart(top, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_text_box_in_chart/#int-int-int-int) | Grafiğe bir metin kutusu ekler.|
| [add_text_effect_in_chart(effect, text, font_name, size, font_bold, font_italic, top, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_text_effect_in_chart/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int) | Grafiğe bir WordArt nesnesi ekler|
| [add_text_effect(effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_text_effect/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int-int-int) | Bir WordArt nesnesi ekler.|
| [add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_word_art/#PresetWordArtStyle-str-int-int-int-int-int-int) | Excel 2007.s'den bu yana hazır WordArt ekler|
| [add_rectangle(upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_rectangle/#int-int-int-int-int-int) | Çalışma sayfasına bir RectangleShape ekler.|
| [add_oval(upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_oval/#int-int-int-int-int-int) | Çalışma sayfasına bir Oval ekler.|
| [add_line(upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_line/#int-int-int-int-int-int) | Çalışma sayfasına bir LineShape ekler.|
| [add_free_floating_shape(type, top, left, height, width, image_data, is_original_size)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/#MsoDrawingType-int-int-int-int-bytes-bool) | Çalışma sayfasına serbest kayan bir şekil ekler. Yalnızca çizgi/görüntü şekli için geçerlidir.|
| [add_arc(upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_arc/#int-int-int-int-int-int) | Çalışma sayfasına bir ArcShape ekler.|
| [add_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_shape/#MsoDrawingType-int-int-int-int-int-int) | Çalışma sayfasına bir Şekil ekler.|
| [add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/#AutoShapeType-int-int-int-int-int-int) | Çalışma sayfasına bir Otomatik Şekil ekler.|
| [add_auto_shape_in_chart(type, top, left, height, width)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_auto_shape_in_chart/#AutoShapeType-int-int-int-int) | Grafiğe bir Otomatik Şekil ekler.|
| [add_active_x_control(type, top_row, top, left_column, left, width, height)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int) | Bir Activex Denetimi oluşturur.|
| [add_svg(upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_svg/#int-int-int-int-int-int-bytes-bytes) | svg görüntüsü ekler.|
| [add_icons(upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_icons/#int-int-int-int-int-int-bytes-bytes) | svg görüntüsü ekler.|
| [add_linked_picture(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_linked_picture/#int-int-int-int-str) | Bağlantılı bir resim ekleyin.|
| [add_ole_object_with_linked_image(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_ole_object_with_linked_image/#int-int-int-int-str) | Bağlantılı bir resim ekleyin.|
| [add_picture_in_chart(top, left, stream, width_scale, height_scale)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_picture_in_chart/#int-int-io.RawIOBase-int-int) | Grafiğe bir resim ekler.|
| [add_ole_object(upper_left_row, top, upper_left_column, left, height, width, image_data)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/add_ole_object/#int-int-int-int-int-int-bytes) | Bir OleObject ekler.|
| [copy_comments_in_range(shapes, ca, dest_row, dest_column)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/copy_comments_in_range/#ShapeCollection-CellArea-int-int) | Aralıktaki tüm yorumları kopyalayın.|
| [copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/copy_in_range/#ShapeCollection-CellArea-int-int-bool) | Aralıktaki şekilleri hedef aralığa kopyalayın.|
| [delete_in_range(ca)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/delete_in_range/#CellArea) | Aralıktaki şekilleri silin. Yorum şekilleri silinmeyecek.|
| [delete_shape(shape)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/delete_shape/#Shape) |Şekil silme Şekil gruptaysa veya bir yorum şekliyse silinmez.|
| [group(group_items)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/group/#list) | Şekilleri gruplandırın.|
| [ungroup(group)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/ungroup/#GroupShape) | Şekil öğelerinin grubunu çözün.|
| [update_selected_value()](/cells/tr/python-net/aspose.cells.drawing/shapecollection/update_selected_value/#) | Seçilen değeri, şekillerin bağlantılı hücresinin değerine göre güncelleyin.|
| [binary_search(item)](/cells/tr/python-net/aspose.cells.drawing/shapecollection/binary_search/#Shape) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|



###  örnekler

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

###  Ayrıca bakınız
* modül [aspose.cells.drawing](..)
