---
title: ShapeCollection
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 530
url: /python-net/aspose.cells.drawing/shapecollection/
---

## ShapeCollection class

Represents all the shape in a worksheet/chart.

The ShapeCollection type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|capacity|  |
## Methods
| Name | Description |
| :- | :- |
|add_shape_in_chart(type, placement, left, top, right, bottom, image_data)|Add a shape to chart .All unit is 1/4000 of chart area.|
|add_shape_in_chart(type, placement, left, top, right, bottom)|Add a shape to chart .All unit is 1/4000 of chart area.|
|add_shape_in_chart_by_scale(type, placement, left, top, right, bottom)|Add a shape to chart. All unit is percent scale of chart area.|
|add_shape_in_chart_by_scale(type, placement, left, top, right, bottom, image_data)|Add a shape to chart .All unit is 1/4000 of chart area.|
|add_picture(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)|Adds a picture to the collection.|
|add_picture(upper_left_row, upper_left_column, stream, width_scale, height_scale)|Adds a picture to the collection.|
|copy_to(array)|  |
|copy_to(index, array, array_index, count)|  |
|index_of(item, index)|  |
|index_of(item, index, count)|  |
|last_index_of(item)|  |
|last_index_of(item, index)|  |
|last_index_of(item, index, count)|  |
|add_copy(source_shape, upper_left_row, top, upper_left_column, left)|Adds and copy a shape to the worksheet.|
|add_check_box(upper_left_row, top, upper_left_column, left, height, width)|Adds a checkbox to the worksheet.|
|add_text_box(upper_left_row, top, upper_left_column, left, height, width)|Adds a text box to the worksheet.|
|add_spinner(upper_left_row, top, upper_left_column, left, height, width)|Adds a Spinner to the worksheet.|
|add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width)|Adds a ScrollBar to the worksheet.|
|add_radio_button(upper_left_row, top, upper_left_column, left, height, width)|Adds a RadioButton to the worksheet.|
|add_list_box(upper_left_row, top, upper_left_column, left, height, width)|Adds a ListBox to the worksheet.|
|add_combo_box(upper_left_row, top, upper_left_column, left, height, width)|Adds a ComboBox to the worksheet.|
|add_group_box(upper_left_row, top, upper_left_column, left, height, width)|Adds a GroupBox to the worksheet.|
|add_button(upper_left_row, top, upper_left_column, left, height, width)|Adds a Button to the worksheet.|
|add_label(upper_left_row, top, upper_left_column, left, height, width)|Adds a Label to the worksheet.|
|add_label_in_chart(top, left, height, width)|Adds a label to the chart.|
|add_text_box_in_chart(top, left, height, width)|Adds a textbox to the chart.|
|add_text_effect_in_chart(effect, text, font_name, size, font_bold, font_italic, top, left, height, width)|Inserts a WordArt object to the chart|
|add_text_effect(effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width)|Inserts a WordArt object to the chart|
|add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width)|Adds preset WordArt since Excel 2007.s|
|add_rectangle(upper_left_row, top, upper_left_column, left, height, width)|Adds a RectangleShape to the worksheet.|
|add_oval(upper_left_row, top, upper_left_column, left, height, width)|Adds a Oval to the worksheet.|
|add_line(upper_left_row, top, upper_left_column, left, height, width)|Adds a LineShape to the worksheet.|
|add_free_floating_shape(type, top, left, height, width, image_data, is_original_size)|Adds a free floating shape to the worksheet.Only applies for line/image shape.|
|add_arc(upper_left_row, top, upper_left_column, left, height, width)|Adds a ArcShape to the worksheet.|
|add_shape(type, upper_left_row, top, upper_left_column, left, height, width)|Add a shape to chart .All unit is 1/4000 of chart area.|
|add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width)|Adds a AutoShape to the worksheet.|
|add_auto_shape_in_chart(type, top, left, height, width)|Adds a AutoShape to the chart.|
|add_active_x_control(type, top_row, top, left_column, left, width, height)|Creates an Activex Control.|
|add_svg(upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data)|Adds svg image.|
|add_icons(upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data)|Adds svg image.|
|add_linked_picture(upper_left_row, upper_left_column, height, width, source_full_name)|Add a linked picture.|
|add_ole_object_with_linked_image(upper_left_row, upper_left_column, height, width, source_full_name)|Add a linked picture.|
|add_picture_in_chart(top, left, stream, width_scale, height_scale)|Adds a picture to the chart.|
|add_ole_object(upper_left_row, top, upper_left_column, left, height, width, image_data)|  |
|copy_comments_in_range(shapes, ca, dest_row, dest_column)|Copy all comments in the range.|
|copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained)|Copy shapes in the range to destination range.|
|delete_in_range(ca)|Delete shapes in the range.Comment shapes will not be deleted.|
|delete_shape(shape)|Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted.|
|group(group_items)|Group the shapes.|
|ungroup(group)|Ungroups the shape items.|
|update_selected_value()|Update the selected value by the value of the linked cell of the shapes.|
|binary_search(item)|  |

### See Also

* namespace [aspose.cells.drawing](/python-net/aspose.cells.drawing/)
* assembly [Aspose.Cells](/python-net/)

