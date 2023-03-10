---
title: ShapeCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 530
url: /ru/python-net/aspose.cells.drawing/shapecollection/
is_root: false
---
##  ShapeCollection класс
Представляет всю форму на листе/диаграмме.



Тип ShapeCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells.drawing/shapecollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add_shape_in_chart(type, placement, left, top, right, bottom, image_data)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int-bytes) | Добавьте фигуру на диаграмму. Все единицы измерения составляют 1/4000 площади диаграммы.|
| [add_shape_in_chart(type, placement, left, top, right, bottom)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int) | Добавьте фигуру на диаграмму. Все единицы измерения составляют 1/4000 площади диаграммы.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float) | Добавьте фигуру на диаграмму. Все единицы измерения представляют собой процентную шкалу области диаграммы.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom, image_data)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float-bytes) | Добавьте фигуру на диаграмму. Все единицы измерения составляют 1/4000 площади диаграммы.|
| [add_picture(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-int-int-io.RawIOBase) | Добавляет изображение в коллекцию.|
| [add_picture(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-io.RawIOBase-int-int) | Добавляет изображение в коллекцию.|
| [copy_to(array)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/copy_to/#int-list-int-int) |Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [add_copy(source_shape, upper_left_row, top, upper_left_column, left)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_copy/#Shape-int-int-int-int) | Добавляет и копирует фигуру на лист.|
| [add_check_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_check_box/#int-int-int-int-int-int) | Добавляет флажок на рабочий лист.|
| [add_text_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_text_box/#int-int-int-int-int-int) | Добавляет текстовое поле на лист.|
| [add_spinner(upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_spinner/#int-int-int-int-int-int) | Добавляет счетчик на рабочий лист.|
| [add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/#int-int-int-int-int-int) | Добавляет полосу прокрутки на рабочий лист.|
| [add_radio_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_radio_button/#int-int-int-int-int-int) | Добавляет RadioButton на лист.|
| [add_list_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_list_box/#int-int-int-int-int-int) | Добавляет ListBox на лист.|
| [add_combo_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_combo_box/#int-int-int-int-int-int) | Добавляет ComboBox на лист.|
| [add_group_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_group_box/#int-int-int-int-int-int) |Добавляет GroupBox на лист.|
| [add_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_button/#int-int-int-int-int-int) | Добавляет кнопку на рабочий лист.|
| [add_label(upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_label/#int-int-int-int-int-int) | Добавляет метку на рабочий лист.|
| [add_label_in_chart(top, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_label_in_chart/#int-int-int-int) | Добавляет метку на диаграмму.|
| [add_text_box_in_chart(top, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_text_box_in_chart/#int-int-int-int) | Добавляет текстовое поле на диаграмму.|
| [add_text_effect_in_chart(effect, text, font_name, size, font_bold, font_italic, top, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_text_effect_in_chart/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int) | Вставляет объект WordArt в диаграмму|
| [add_text_effect(effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_text_effect/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int-int-int) | Вставляет объект WordArt.|
| [add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_word_art/#PresetWordArtStyle-str-int-int-int-int-int-int) | Добавляет предустановленные WordArt начиная с Excel 2007.s|
| [add_rectangle(upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_rectangle/#int-int-int-int-int-int) | Добавляет RectangleShape на рабочий лист.|
| [add_oval(upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_oval/#int-int-int-int-int-int) | Добавляет овал на рабочий лист.|
| [add_line(upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_line/#int-int-int-int-int-int) | Добавляет LineShape на лист.|
| [add_free_floating_shape(type, top, left, height, width, image_data, is_original_size)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/#MsoDrawingType-int-int-int-int-bytes-bool) | Добавляет на лист свободно плавающую фигуру. Применяется только для формы линии/изображения.|
| [add_arc(upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_arc/#int-int-int-int-int-int) | Добавляет ArcShape на рабочий лист.|
| [add_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_shape/#MsoDrawingType-int-int-int-int-int-int) | Добавляет фигуру на лист.|
| [add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/#AutoShapeType-int-int-int-int-int-int) | Добавляет автофигуру на лист.|
| [add_auto_shape_in_chart(type, top, left, height, width)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_auto_shape_in_chart/#AutoShapeType-int-int-int-int) | Добавляет автофигуру на диаграмму.|
| [add_active_x_control(type, top_row, top, left_column, left, width, height)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int) | Создает элемент управления Activex.|
| [add_svg(upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_svg/#int-int-int-int-int-int-bytes-bytes) | Добавляет SVG-изображение.|
| [add_icons(upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_icons/#int-int-int-int-int-int-bytes-bytes) | Добавляет SVG-изображение.|
| [add_linked_picture(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_linked_picture/#int-int-int-int-str) | Добавьте связанное изображение.|
| [add_ole_object_with_linked_image(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_ole_object_with_linked_image/#int-int-int-int-str) | Добавьте связанное изображение.|
| [add_picture_in_chart(top, left, stream, width_scale, height_scale)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_picture_in_chart/#int-int-io.RawIOBase-int-int) | Добавляет изображение на диаграмму.|
| [add_ole_object(upper_left_row, top, upper_left_column, left, height, width, image_data)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/add_ole_object/#int-int-int-int-int-int-bytes) | Добавляет OleObject.|
| [copy_comments_in_range(shapes, ca, dest_row, dest_column)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/copy_comments_in_range/#ShapeCollection-CellArea-int-int) | Скопируйте все комментарии в диапазоне.|
| [copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/copy_in_range/#ShapeCollection-CellArea-int-int-bool) | Скопируйте фигуры из диапазона в целевой диапазон.|
| [delete_in_range(ca)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/delete_in_range/#CellArea) | Удалить фигуры в диапазоне. Фигуры комментариев не будут удалены.|
| [delete_shape(shape)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/delete_shape/#Shape) |Удалить фигуру. Если фигура находится в группе или является фигурой комментария, она не будет удалена.|
| [group(group_items)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/group/#list) | Сгруппируйте фигуры.|
| [ungroup(group)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/ungroup/#GroupShape) | Разгруппирует элементы формы.|
| [update_selected_value()](/cells/ru/python-net/aspose.cells.drawing/shapecollection/update_selected_value/#) | Обновите выбранное значение значением связанной ячейки фигур.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells.drawing/shapecollection/binary_search/#Shape) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Пример

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

###  Смотрите также
* модуль [aspose.cells.drawing](..)
