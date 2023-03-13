---
title: ShapeCollection类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 530
url: /zh/python-net/aspose.cells.drawing/shapecollection/
is_root: false
---
## ShapeCollection类
代表工作表/图表中的所有形状。



ShapeCollection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [capacity](/cells/zh/python-net/aspose.cells.drawing/shapecollection/capacity) |获取或设置数组列表可以包含的元素数。|


### 方法
|方法|描述|
| :- | :- |
| [add_shape_in_chart(type, placement, left, top, right, bottom, image_data)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int-bytes) |添加图形到图表。所有单位是图表面积的 1/4000。|
| [add_shape_in_chart(type, placement, left, top, right, bottom)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int) |添加图形到图表。所有单位是图表面积的 1/4000。|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float) |向图表添加形状。所有单位都是图表区域的百分比比例。|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom, image_data)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float-bytes) |添加图形到图表。所有单位是图表面积的 1/4000。|
| [add_picture(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-int-int-io.RawIOBase) |将图片添加到集合中。|
| [add_picture(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-io.RawIOBase-int-int) |将图片添加到集合中。|
| [copy_to(array)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/copy_to/#list) |将整个数组列表复制到兼容的一维数组列表，从目标数组列表的开头开始。|
| [copy_to(index, array, array_index, count)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/copy_to/#int-list-int-int) |将数组列表中的一系列元素复制到兼容的一维数组列表，从目标数组列表的指定索引开始。|
| [index_of(item, index)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int) |搜索指定的对象并返回数组列表中从指定索引延伸到最后一个元素的元素范围内第一次出现的从零开始的索引。|
| [index_of(item, index, count)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int-int) |搜索指定的对象并返回数组列表中从指定索引开始并包含指定数量的元素的元素范围内第一次出现的从零开始的索引。|
| [last_index_of(item)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape) |搜索指定的对象并返回整个数组列表中最后一次出现的从零开始的索引。|
| [last_index_of(item, index)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int) |搜索指定的对象并返回数组列表中从第一个元素到指定索引的元素范围内最后一次出现的从零开始的索引。|
| [last_index_of(item, index, count)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int-int) |搜索指定的对象并返回数组列表中包含指定数量的元素并以指定索引结束的元素范围内最后一次出现的从零开始的索引。|
| [add_copy(source_shape, upper_left_row, top, upper_left_column, left)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_copy/#Shape-int-int-int-int) |添加形状并将其复制到工作表。|
| [add_check_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_check_box/#int-int-int-int-int-int) |向工作表添加一个复选框。|
| [add_text_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_text_box/#int-int-int-int-int-int) |向工作表添加文本框。|
| [add_spinner(upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_spinner/#int-int-int-int-int-int) |将微调器添加到工作表。|
| [add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/#int-int-int-int-int-int) |将 ScrollBar 添加到工作表。|
| [add_radio_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_radio_button/#int-int-int-int-int-int) |将 RadioButton 添加到工作表。|
| [add_list_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_list_box/#int-int-int-int-int-int) |将 ListBox 添加到工作表。|
| [add_combo_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_combo_box/#int-int-int-int-int-int) |将 ComboBox 添加到工作表。|
| [add_group_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_group_box/#int-int-int-int-int-int) |将 GroupBox 添加到工作表。|
| [add_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_button/#int-int-int-int-int-int) |向工作表添加一个按钮。|
| [add_label(upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_label/#int-int-int-int-int-int) |向工作表添加标签。|
| [add_label_in_chart(top, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_label_in_chart/#int-int-int-int) |向图表添加标签。|
| [add_text_box_in_chart(top, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_text_box_in_chart/#int-int-int-int) |向图表添加文本框。|
| [add_text_effect_in_chart(effect, text, font_name, size, font_bold, font_italic, top, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_text_effect_in_chart/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int) |将艺术字对象插入图表|
| [add_text_effect(effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_text_effect/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int-int-int) |插入艺术字对象。|
| [add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_word_art/#PresetWordArtStyle-str-int-int-int-int-int-int) |自 Excel 2007.s 起添加预设艺术字|
| [add_rectangle(upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_rectangle/#int-int-int-int-int-int) |将 RectangleShape 添加到工作表。|
| [add_oval(upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_oval/#int-int-int-int-int-int) |向工作表添加椭圆。|
| [add_line(upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_line/#int-int-int-int-int-int) |将 LineShape 添加到工作表。|
| [add_free_floating_shape(type, top, left, height, width, image_data, is_original_size)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/#MsoDrawingType-int-int-int-int-bytes-bool) |向工作表添加自由浮动形状。仅适用于线条/图像形状。|
| [add_arc(upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_arc/#int-int-int-int-int-int) |将 ArcShape 添加到工作表。|
| [add_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_shape/#MsoDrawingType-int-int-int-int-int-int) |将形状添加到工作表。|
| [add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/#AutoShapeType-int-int-int-int-int-int) |将自选图形添加到工作表。|
| [add_auto_shape_in_chart(type, top, left, height, width)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_auto_shape_in_chart/#AutoShapeType-int-int-int-int) |向图表添加自选图形。|
| [add_active_x_control(type, top_row, top, left_column, left, width, height)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int) |创建一个 Activex 控件。|
| [add_svg(upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_svg/#int-int-int-int-int-int-bytes-bytes) |添加 svg 图像。|
| [add_icons(upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_icons/#int-int-int-int-int-int-bytes-bytes) |添加 svg 图像。|
| [add_linked_picture(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_linked_picture/#int-int-int-int-str) |添加链接图片。|
| [add_ole_object_with_linked_image(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_ole_object_with_linked_image/#int-int-int-int-str) |添加链接图片。|
| [add_picture_in_chart(top, left, stream, width_scale, height_scale)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_picture_in_chart/#int-int-io.RawIOBase-int-int) |向图表添加图片。|
| [add_ole_object(upper_left_row, top, upper_left_column, left, height, width, image_data)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/add_ole_object/#int-int-int-int-int-int-bytes) |添加一个 OleObject。|
| [copy_comments_in_range(shapes, ca, dest_row, dest_column)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/copy_comments_in_range/#ShapeCollection-CellArea-int-int) |复制范围内的所有评论。|
| [copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/copy_in_range/#ShapeCollection-CellArea-int-int-bool) |将范围内的形状复制到目标范围。|
| [delete_in_range(ca)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/delete_in_range/#CellArea) |删除范围内的形状。注释形状不会被删除。|
| [delete_shape(shape)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/delete_shape/#Shape) |删除形状。如果形状在组中或者是评论形状，则不会被删除。|
| [group(group_items)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/group/#list) |对形状进行分组。|
| [ungroup(group)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/ungroup/#GroupShape) |取消组合形状项目。|
| [update_selected_value()](/cells/zh/python-net/aspose.cells.drawing/shapecollection/update_selected_value/#) |通过形状的链接单元格的值更新所选值。|
| [binary_search(item)](/cells/zh/python-net/aspose.cells.drawing/shapecollection/binary_search/#Shape) |使用默认比较器在整个排序数组列表中搜索元素，并返回元素的从零开始的索引。|



### 例子

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

### 也可以看看
* 模块 [aspose.cells.drawing](..)
