---
title: ShapeCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 530
url: /ar/python-net/aspose.cells.drawing/shapecollection/
is_root: false
---
##  ShapeCollection الدرجة
يمثل جميع الأشكال في ورقة عمل / مخطط.



يكشف نوع ShapeCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [capacity](/cells/ar/python-net/aspose.cells.drawing/shapecollection/capacity) | الحصول على أو تحديد عدد العناصر التي يمكن أن تحتويها قائمة الصفيف.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [add_shape_in_chart(type, placement, left, top, right, bottom, image_data)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int-bytes) | أضف شكلاً إلى الرسم البياني. جميع الوحدات هي 1/4000 من منطقة المخطط.|
| [add_shape_in_chart(type, placement, left, top, right, bottom)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int) | أضف شكلاً إلى الرسم البياني. جميع الوحدات هي 1/4000 من منطقة المخطط.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float) | أضف شكلاً إلى المخطط. جميع الوحدات هي مقياس نسبة مئوية من منطقة المخطط.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom, image_data)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float-bytes) | أضف شكلاً إلى الرسم البياني. جميع الوحدات هي 1/4000 من منطقة المخطط.|
| [add_picture(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-int-int-io.RawIOBase) | يضيف صورة إلى المجموعة.|
| [add_picture(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-io.RawIOBase-int-int) | يضيف صورة إلى المجموعة.|
| [copy_to(array)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/copy_to/#list) | ينسخ قائمة المصفوفات بأكملها إلى قائمة مصفوفة متوافقة أحادية البعد ، بدءًا من بداية قائمة الصفيف الهدف.|
| [copy_to(index, array, array_index, count)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/copy_to/#int-list-int-int) |ينسخ نطاقًا من العناصر من قائمة المصفوفة إلى قائمة مصفوفة أحادية البعد متوافقة ، بدءًا من الفهرس المحدد لقائمة الصفيف الهدف.|
| [index_of(item, index)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من الفهرس المحدد إلى العنصر الأخير.|
| [index_of(item, index, count)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يبدأ بالفهرس المحدد ويحتوي على عدد محدد من العناصر.|
| [last_index_of(item)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأخير ضمن قائمة الصفيف بأكملها.|
| [last_index_of(item, index)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int) | يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من العنصر الأول إلى الفهرس المحدد.|
| [last_index_of(item, index, count)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int-int) |يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف التي تحتوي على عدد محدد من العناصر وتنتهي عند الفهرس المحدد.|
| [add_copy(source_shape, upper_left_row, top, upper_left_column, left)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_copy/#Shape-int-int-int-int) | يضيف شكلاً وينسخه إلى ورقة العمل.|
| [add_check_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_check_box/#int-int-int-int-int-int) | يضيف مربع اختيار إلى ورقة العمل.|
| [add_text_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_text_box/#int-int-int-int-int-int) | يضيف مربع نص إلى ورقة العمل.|
| [add_spinner(upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_spinner/#int-int-int-int-int-int) | يضيف Spinner إلى ورقة العمل.|
| [add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/#int-int-int-int-int-int) | يضيف شريط تمرير إلى ورقة العمل.|
| [add_radio_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_radio_button/#int-int-int-int-int-int) | يضيف RadioButton إلى ورقة العمل.|
| [add_list_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_list_box/#int-int-int-int-int-int) | يضيف ListBox إلى ورقة العمل.|
| [add_combo_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_combo_box/#int-int-int-int-int-int) | يضيف ComboBox إلى ورقة العمل.|
| [add_group_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_group_box/#int-int-int-int-int-int) |يضيف GroupBox إلى ورقة العمل.|
| [add_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_button/#int-int-int-int-int-int) | يضيف زرًا إلى ورقة العمل.|
| [add_label(upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_label/#int-int-int-int-int-int) | يضيف تسمية إلى ورقة العمل.|
| [add_label_in_chart(top, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_label_in_chart/#int-int-int-int) | يضيف تسمية إلى المخطط.|
| [add_text_box_in_chart(top, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_text_box_in_chart/#int-int-int-int) | يضيف مربع نص إلى الرسم البياني.|
| [add_text_effect_in_chart(effect, text, font_name, size, font_bold, font_italic, top, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_text_effect_in_chart/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int) | إدراج كائن WordArt في المخطط|
| [add_text_effect(effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_text_effect/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int-int-int) | يُدرج كائن WordArt.|
| [add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_word_art/#PresetWordArtStyle-str-int-int-int-int-int-int) | يضيف WordArt المعين مسبقًا منذ Excel 2007.s|
| [add_rectangle(upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_rectangle/#int-int-int-int-int-int) | يضيف RectangleShape إلى ورقة العمل.|
| [add_oval(upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_oval/#int-int-int-int-int-int) | يضيف شكل بيضوي إلى ورقة العمل.|
| [add_line(upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_line/#int-int-int-int-int-int) | يضيف LineShape إلى ورقة العمل.|
| [add_free_floating_shape(type, top, left, height, width, image_data, is_original_size)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/#MsoDrawingType-int-int-int-int-bytes-bool) | يضيف شكلاً عائمًا حرًا إلى ورقة العمل. ينطبق فقط على شكل الخط / الصورة.|
| [add_arc(upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_arc/#int-int-int-int-int-int) | يضيف شكل ArcShape إلى ورقة العمل.|
| [add_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_shape/#MsoDrawingType-int-int-int-int-int-int) | يضيف شكلاً إلى ورقة العمل.|
| [add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/#AutoShapeType-int-int-int-int-int-int) | يضيف شكلاً تلقائيًا إلى ورقة العمل.|
| [add_auto_shape_in_chart(type, top, left, height, width)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_auto_shape_in_chart/#AutoShapeType-int-int-int-int) | يضيف شكلاً تلقائيًا إلى المخطط.|
| [add_active_x_control(type, top_row, top, left_column, left, width, height)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int) | ينشئ عنصر تحكم Activex.|
| [add_svg(upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_svg/#int-int-int-int-int-int-bytes-bytes) | يضيف صورة svg.|
| [add_icons(upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_icons/#int-int-int-int-int-int-bytes-bytes) | يضيف صورة svg.|
| [add_linked_picture(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_linked_picture/#int-int-int-int-str) | أضف صورة مرتبطة.|
| [add_ole_object_with_linked_image(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_ole_object_with_linked_image/#int-int-int-int-str) | أضف صورة مرتبطة.|
| [add_picture_in_chart(top, left, stream, width_scale, height_scale)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_picture_in_chart/#int-int-io.RawIOBase-int-int) | يضيف صورة إلى المخطط.|
| [add_ole_object(upper_left_row, top, upper_left_column, left, height, width, image_data)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/add_ole_object/#int-int-int-int-int-int-bytes) | يضيف OleObject.|
| [copy_comments_in_range(shapes, ca, dest_row, dest_column)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/copy_comments_in_range/#ShapeCollection-CellArea-int-int) | انسخ جميع التعليقات في النطاق.|
| [copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/copy_in_range/#ShapeCollection-CellArea-int-int-bool) | انسخ الأشكال الموجودة في النطاق إلى النطاق الوجهة.|
| [delete_in_range(ca)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/delete_in_range/#CellArea) | احذف الأشكال في النطاق. لن يتم حذف أشكال التعليقات.|
| [delete_shape(shape)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/delete_shape/#Shape) |حذف شكل. إذا كان الشكل في المجموعة أو شكل تعليق ، فلن يتم حذفه.|
| [group(group_items)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/group/#list) | اجمع الأشكال.|
| [ungroup(group)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/ungroup/#GroupShape) | فك تجميع عناصر الشكل.|
| [update_selected_value()](/cells/ar/python-net/aspose.cells.drawing/shapecollection/update_selected_value/#) | قم بتحديث القيمة المحددة بقيمة الخلية المرتبطة بالأشكال.|
| [binary_search(item)](/cells/ar/python-net/aspose.cells.drawing/shapecollection/binary_search/#Shape) | يبحث في قائمة الصفيف التي تم فرزها بالكامل عن عنصر باستخدام المقارنة الافتراضية ويعيد فهرس العنصر على أساس الصفر.|



###  أمثلة

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

###  أنظر أيضا
* وحدة [aspose.cells.drawing](..)
