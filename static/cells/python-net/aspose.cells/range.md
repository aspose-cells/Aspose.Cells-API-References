##Range class
## Range class
Encapsulates the object that represents a range of cells within a spreadsheet.
The Range type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [current_region](/cells/python-net/aspose.cells/range/current_region) | Returns a Range object that represents the current region.
| [hyperlinks](/cells/python-net/aspose.cells/range/hyperlinks) | Gets all hyperlink in the range. |
| [row_count](/cells/python-net/aspose.cells/range/row_count) | Gets the count of rows in the range. |
| [column_count](/cells/python-net/aspose.cells/range/column_count) | Gets the count of columns in the range. |
| [name](/cells/python-net/aspose.cells/range/name) | Gets or sets the name of the range. |
| [refers_to](/cells/python-net/aspose.cells/range/refers_to) | Gets the range's refers to. |
| [address](/cells/python-net/aspose.cells/range/address) | Gets address of the range. |
| [left](/cells/python-net/aspose.cells/range/left) | Gets the distance, in points, from the left edge of column A to the left edge of the range. |
| [top](/cells/python-net/aspose.cells/range/top) | Gets the distance, in points, from the top edge of row 1 to the top edge of the range. |
| [width](/cells/python-net/aspose.cells/range/width) | Gets the width of a range in points. |
| [height](/cells/python-net/aspose.cells/range/height) | Gets the width of a range in points. |
| [first_row](/cells/python-net/aspose.cells/range/first_row) | Gets the index of the first row of the range. |
| [first_column](/cells/python-net/aspose.cells/range/first_column) | Gets the index of the first column of the range. |
| [value](/cells/python-net/aspose.cells/range/value) | Gets and sets the value of the range. |
| [column_width](/cells/python-net/aspose.cells/range/column_width) | Sets or gets the column width of this range |
| [row_height](/cells/python-net/aspose.cells/range/row_height) | Sets or gets the height of rows in this range |
| [entire_column](/cells/python-net/aspose.cells/range/entire_column) | Gets a Range object that represents the entire column (or columns) that contains the specified range. |
| [entire_row](/cells/python-net/aspose.cells/range/entire_row) | Gets a Range object that represents the entire row (or rows) that contains the specified range. |
| [worksheet](/cells/python-net/aspose.cells/range/worksheet) | Gets the [`Range.worksheet`](/cells/python-net/aspose.cells/range#worksheet)object which contains this range. |
### Methods
| Method | Description |
| :- | :- |
| [`auto_fill(self, target)`](/cells/python-net/aspose.cells/range/auto_fill/#aspose.cells.range) | Automaticall fill the target range. |
| [`auto_fill(self, target, auto_fill_type)`](/cells/python-net/aspose.cells/range/auto_fill/#aspose.cells.range-aspose.cells.autofilltype) | Automaticall fill the target range. |
| [`set_style(self, style, explicit_flag)`](/cells/python-net/aspose.cells/range/set_style/#aspose.cells.style-bool) | Apply the cell style. |
| [`set_style(self, style)`](/cells/python-net/aspose.cells/range/set_style/#aspose.cells.style) | Sets the style of the range. |
| [`set_outline_borders(self, border_style, border_color)`](/cells/python-net/aspose.cells/range/set_outline_borders/#aspose.cells.cellbordertype-aspose.cells.cellscolor) | Sets the outline borders around a range of cells with same border style and color. |
| [`set_outline_borders(self, border_style, border_color)`](/cells/python-net/aspose.cells/range/set_outline_borders/#aspose.cells.cellbordertype-aspose.pydrawing.color) | Sets the outline borders around a range of cells with same border style and color. |
| [`set_outline_borders(self, border_styles, border_colors)`](/cells/python-net/aspose.cells/range/set_outline_borders/#list-aspose.pydrawing.color[]) | Sets out line borders around a range of cells. |
| [`set_outline_border(self, border_edge, border_style, border_color)`](/cells/python-net/aspose.cells/range/set_outline_border/#aspose.cells.bordertype-aspose.cells.cellbordertype-aspose.cells.cellscolor) | Sets outline border around a range of cells. |
| [`set_outline_border(self, border_edge, border_style, border_color)`](/cells/python-net/aspose.cells/range/set_outline_border/#aspose.cells.bordertype-aspose.cells.cellbordertype-aspose.pydrawing.color) | Sets outline border around a range of cells. |
| [`copy(self, range, options)`](/cells/python-net/aspose.cells/range/copy/#aspose.cells.range-aspose.cells.pasteoptions) | Copying the range with paste special options. |
| [`copy(self, range)`](/cells/python-net/aspose.cells/range/copy/#aspose.cells.range) | Copies data (including formulas), formatting, drawing objects etc. from a source range. |
| [`add_hyperlink(self, address, text_to_display, screen_tip)`](/cells/python-net/aspose.cells/range/add_hyperlink/#system.string-system.string-system.string) | Adds a hyperlink to a specified cell or a range of cells. |
| [`is_intersect(self, range)`](/cells/python-net/aspose.cells/range/is_intersect/#aspose.cells.range) | Indicates whether the range is intersect. |
| [`intersect(self, range)`](/cells/python-net/aspose.cells/range/intersect/#aspose.cells.range) | Returns a [`Range`](/cells/python-net/aspose.cells/range) object that represents the rectangular intersection of two ranges. |
| [`union_rang(self, range)`](/cells/python-net/aspose.cells/range/union_rang/#aspose.cells.range) | Returns the union result of two ranges. |
| [`union_ranges(self, ranges)`](/cells/python-net/aspose.cells/range/union_ranges/#list) | Returns the union result of two ranges. |
| [`union(self, range)`](/cells/python-net/aspose.cells/range/union/#aspose.cells.range) | Returns the union of two ranges. |
| [`is_blank(self)`](/cells/python-net/aspose.cells/range/is_blank/#) | Indicates whether the range contains values. |
| [`merge(self)`](/cells/python-net/aspose.cells/range/merge/#) | Combines a range of cells into a single cell. |
| [`un_merge(self)`](/cells/python-net/aspose.cells/range/un_merge/#) | Unmerges merged cells of this range. |
| [`put_value(self, string_value, is_converted, set_style)`](/cells/python-net/aspose.cells/range/put_value/#system.string-bool-bool) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [`apply_style(self, style, flag)`](/cells/python-net/aspose.cells/range/apply_style/#aspose.cells.style-aspose.cells.styleflag) | Applies formats for a whole range. |
| [`set_inside_borders(self, border_edge, line_style, border_color)`](/cells/python-net/aspose.cells/range/set_inside_borders/#aspose.cells.bordertype-aspose.cells.cellbordertype-aspose.cells.cellscolor) | Set inside borders of the range. |
| [`move_to(self, dest_row, dest_column)`](/cells/python-net/aspose.cells/range/move_to/#int-int) | Move the current range to the dest range. |
| [`copy_data(self, range)`](/cells/python-net/aspose.cells/range/copy_data/#aspose.cells.range) | Copies cell data (including formulas) from a source range. |
| [`copy_value(self, range)`](/cells/python-net/aspose.cells/range/copy_value/#aspose.cells.range) | Copies cell value from a source range. |
| [`copy_style(self, range)`](/cells/python-net/aspose.cells/range/copy_style/#aspose.cells.range) | Copies style settings from a source range. |
| [`transpose(self)`](/cells/python-net/aspose.cells/range/transpose/#) | Transpose (rotate) data from rows to columns or vice versa. |
| [`get(self, row_offset, column_offset)`](/cells/python-net/aspose.cells/range/get/#int-int) | Add API for Python Via .Net.since this[int, int] is unsupported |
| [`get_cell_or_null(self, row_offset, column_offset)`](/cells/python-net/aspose.cells/range/get_cell_or_null/#int-int) | Gets [`Cell`](/cells/python-net/aspose.cells/cell) object or null in this range. |
| [`get_offset(self, row_offset, column_offset)`](/cells/python-net/aspose.cells/range/get_offset/#int-int) | Gets [`Range`](/cells/python-net/aspose.cells/range) range by offset. |
| [`to_image(self, options)`](/cells/python-net/aspose.cells/range/to_image/#aspose.cells.rendering.imageorprintoptions) | Converts the range to image. |
| [`to_json(self, options)`](/cells/python-net/aspose.cells/range/to_json/#aspose.cells.jsonsaveoptions) | Convert the range to JSON value. |
| [`to_html(self, save_options)`](/cells/python-net/aspose.cells/range/to_html/#aspose.cells.htmlsaveoptions) | Convert the range to html . |
| [`clear(self)`](/cells/python-net/aspose.cells/range/clear/#) | Clears this range. |
| [`clear_contents(self)`](/cells/python-net/aspose.cells/range/clear_contents/#) | Clears the contents of this range. |
| [`clear_formats(self)`](/cells/python-net/aspose.cells/range/clear_formats/#) | Clears the formats of this range. |
| [`clear_comments(self)`](/cells/python-net/aspose.cells/range/clear_comments/#) | Clears the comments of this range. |
| [`clear_hyperlinks(self, clear_format)`](/cells/python-net/aspose.cells/range/clear_hyperlinks/#bool) | Only removes hyperlinks. |
### Remarks
The Range class denotes a region of Excel spreadsheet.
With this, you can format and set value of the range.
And you can simply copy range of Excel too.
### Example
The following example shows how to create a range and set value the range of Excel.
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
#  Create a range (A1:D3).
range = cells.create_range("A1", "D3")
#  Set value to the range.
range.value = "Hello"
# Save the Excel file
workbook.save("book1.xlsm")
```
### See Also
* module [`aspose.cells`](..)
* class [`Cell`](/cells/python-net/aspose.cells/cell)
* class [`Range`](/cells/python-net/aspose.cells/range)
