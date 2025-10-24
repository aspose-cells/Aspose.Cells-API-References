##ShapeCollection class
## ShapeCollection class
Represents all the shape in a worksheet/chart.
The ShapeCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells.drawing/shapecollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`add_shape_in_chart(self, type, placement, left, top, right, bottom, image_data)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#aspose.cells.drawing.msodrawingtype-aspose.cells.drawing.placementtype-int-int-int-int-bytes) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [`add_shape_in_chart(self, type, placement, left, top, right, bottom)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#aspose.cells.drawing.msodrawingtype-aspose.cells.drawing.placementtype-int-int-int-int) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [`add_shape_in_chart_by_scale(self, type, placement, left, top, right, bottom)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#aspose.cells.drawing.msodrawingtype-aspose.cells.drawing.placementtype-float-float-float-float) | Add a shape to chart. All unit is percent scale of chart area. |
| [`add_shape_in_chart_by_scale(self, type, placement, left, top, right, bottom, image_data)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#aspose.cells.drawing.msodrawingtype-aspose.cells.drawing.placementtype-float-float-float-float-bytes) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [`add_picture(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-int-int-io.rawiobase) | Adds a picture to the collection. |
| [`add_picture(self, upper_left_row, upper_left_column, stream, width_scale, height_scale)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-io.rawiobase-int-int) | Adds a picture to the collection. |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells.drawing/shapecollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells.drawing/shapecollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells.drawing/shapecollection/index_of/#aspose.cells.drawing.shape-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells.drawing/shapecollection/index_of/#aspose.cells.drawing.shape-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells.drawing/shapecollection/last_index_of/#aspose.cells.drawing.shape) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells.drawing/shapecollection/last_index_of/#aspose.cells.drawing.shape-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells.drawing/shapecollection/last_index_of/#aspose.cells.drawing.shape-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`get(self, name)`](/cells/python-net/aspose.cells.drawing/shapecollection/get/#system.string) | Gets the [`Shape`](/cells/python-net/aspose.cells.drawing/shape) object by the name of the shape. |
| [`add_copy(self, source_shape, top_row, top, left_column, left)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_copy/#aspose.cells.drawing.shape-int-int-int-int) | Adds and copy a shape to the worksheet. |
| [`add_check_box(self, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_check_box/#int-int-int-int-int-int) | Adds a checkbox to the worksheet. |
| [`add_text_box(self, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_text_box/#int-int-int-int-int-int) | Adds a text box to the worksheet. |
| [`add_equation(self, top_row, top, left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_equation/#int-int-int-int-int-int) | Add an equation object to the worksheet. |
| [`add_spinner(self, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_spinner/#int-int-int-int-int-int) | Adds a Spinner to the worksheet. |
| [`add_scroll_bar(self, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/#int-int-int-int-int-int) | Adds a ScrollBar to the worksheet. |
| [`add_radio_button(self, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_radio_button/#int-int-int-int-int-int) | Adds a RadioButton to the worksheet. |
| [`add_list_box(self, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_list_box/#int-int-int-int-int-int) | Adds a ListBox to the worksheet. |
| [`add_combo_box(self, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_combo_box/#int-int-int-int-int-int) | Adds a ComboBox to the worksheet. |
| [`add_group_box(self, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_group_box/#int-int-int-int-int-int) | Adds a GroupBox to the worksheet. |
| [`add_button(self, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_button/#int-int-int-int-int-int) | Adds a Button to the worksheet. |
| [`add_label(self, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_label/#int-int-int-int-int-int) | Adds a Label to the worksheet. |
| [`add_label_in_chart(self, top, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_label_in_chart/#int-int-int-int) | Adds a label to the chart. |
| [`add_text_box_in_chart(self, top, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_text_box_in_chart/#int-int-int-int) | Adds a textbox to the chart. |
| [`add_text_effect_in_chart(self, effect, text, font_name, size, font_bold, font_italic, top, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_text_effect_in_chart/#aspose.cells.drawing.msopresettexteffect-system.string-system.string-int-bool-bool-int-int-int-int) | Inserts a WordArt object to the chart |
| [`add_text_effect(self, effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_text_effect/#aspose.cells.drawing.msopresettexteffect-system.string-system.string-int-bool-bool-int-int-int-int-int-int) | Inserts a WordArt object. |
| [`add_word_art(self, style, text, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_word_art/#aspose.cells.drawing.presetwordartstyle-system.string-int-int-int-int-int-int) | Adds preset WordArt since Excel 2007.s |
| [`add_rectangle(self, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_rectangle/#int-int-int-int-int-int) | Adds a RectangleShape to the worksheet. |
| [`add_oval(self, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_oval/#int-int-int-int-int-int) | Adds a Oval to the worksheet. |
| [`add_line(self, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_line/#int-int-int-int-int-int) | Adds a LineShape to the worksheet. |
| [`add_free_floating_shape(self, type, top, left, height, width, image_data, is_original_size)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/#aspose.cells.drawing.msodrawingtype-int-int-int-int-bytes-bool) | Adds a free floating shape to the worksheet.Only applies for line/image shape. |
| [`add_arc(self, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_arc/#int-int-int-int-int-int) | Adds a ArcShape to the worksheet. |
| [`add_shape(self, type, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_shape/#aspose.cells.drawing.msodrawingtype-int-int-int-int-int-int) | Adds a Shape to the worksheet. |
| [`add_auto_shape(self, type, upper_left_row, top, upper_left_column, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/#aspose.cells.drawing.autoshapetype-int-int-int-int-int-int) | Adds a AutoShape to the worksheet. |
| [`add_auto_shape_in_chart(self, type, top, left, height, width)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_auto_shape_in_chart/#aspose.cells.drawing.autoshapetype-int-int-int-int) | Adds a AutoShape to the chart. |
| [`add_active_x_control(self, type, top_row, top, left_column, left, width, height)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/#aspose.cells.drawing.activexcontrols.controltype-int-int-int-int-int-int) | Creates an Activex Control. |
| [`add_svg(self, upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_svg/#int-int-int-int-int-int-bytes-bytes) | Adds svg image. |
| [`add_icons(self, upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_icons/#int-int-int-int-int-int-bytes-bytes) | Adds svg image. |
| [`add_linked_picture(self, upper_left_row, upper_left_column, height, width, source_full_name)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_linked_picture/#int-int-int-int-system.string) | Add a linked picture. |
| [`add_ole_object_with_linked_image(self, upper_left_row, upper_left_column, height, width, source_full_name)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_ole_object_with_linked_image/#int-int-int-int-system.string) | Add a linked picture. |
| [`add_picture_in_chart(self, top, left, stream, width_scale, height_scale)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_picture_in_chart/#int-int-io.rawiobase-int-int) | Adds a picture to the chart. |
| [`add_ole_object(self, upper_left_row, top, upper_left_column, left, height, width, image_data)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_ole_object/#int-int-int-int-int-int-bytes) | Adds an OleObject. |
| [`copy_comments_in_range(self, shapes, ca, dest_row, dest_column)`](/cells/python-net/aspose.cells.drawing/shapecollection/copy_comments_in_range/#aspose.cells.drawing.shapecollection-aspose.cells.cellarea-int-int) | Copy all comments in the range. |
| [`copy_in_range(self, source_shapes, ca, dest_row, dest_column, is_contained)`](/cells/python-net/aspose.cells.drawing/shapecollection/copy_in_range/#aspose.cells.drawing.shapecollection-aspose.cells.cellarea-int-int-bool) | Copy shapes in the range to destination range. |
| [`delete_in_range(self, ca)`](/cells/python-net/aspose.cells.drawing/shapecollection/delete_in_range/#aspose.cells.cellarea) | Delete shapes in the range.Comment shapes will not be deleted. |
| [`delete_shape(self, shape)`](/cells/python-net/aspose.cells.drawing/shapecollection/delete_shape/#aspose.cells.drawing.shape) | Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted. |
| [`group(self, group_items)`](/cells/python-net/aspose.cells.drawing/shapecollection/group/#list) | Group the shapes. |
| [`ungroup(self, group)`](/cells/python-net/aspose.cells.drawing/shapecollection/ungroup/#aspose.cells.drawing.groupshape) | Ungroups the shape items. |
| [`remove_a_shape(self, shape)`](/cells/python-net/aspose.cells.drawing/shapecollection/remove_a_shape/#aspose.cells.drawing.shape) | Add API for Python Via .Net.since this API is unsupported |
| [`update_selected_value(self)`](/cells/python-net/aspose.cells.drawing/shapecollection/update_selected_value/#) | Update the selected value by the value of the linked cell or range of the shape. |
| [`add_freeform(self, upper_left_row, top, upper_left_column, left, height, width, paths)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_freeform/#int-int-int-int-int-int-list) | Adds a freeform shape to the worksheet. |
| [`add_signature_line(self, upper_left_row, upper_left_column, signature_line)`](/cells/python-net/aspose.cells.drawing/shapecollection/add_signature_line/#int-int-aspose.cells.drawing.signatureline) | Adds a Signature Line to the worksheet. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells.drawing/shapecollection/binary_search/#aspose.cells.drawing.shape) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### Example
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
### See Also
* module [`aspose.cells.drawing`](..)
* class [`Shape`](/cells/python-net/aspose.cells.drawing/shape)
