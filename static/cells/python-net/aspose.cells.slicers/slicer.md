##Slicer class
## Slicer class
summary description of Slicer View
The Slicer type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [title](/cells/python-net/aspose.cells.slicers/slicer/title) | Specifies the title of the current Slicer object. |
| [alternative_text](/cells/python-net/aspose.cells.slicers/slicer/alternative_text) | Returns or sets the descriptive (alternative) text string of the Slicer object. |
| [is_printable](/cells/python-net/aspose.cells.slicers/slicer/is_printable) | Indicates whether the slicer object is printable. |
| [is_locked](/cells/python-net/aspose.cells.slicers/slicer/is_locked) | Indicates whether the slicer shape is locked. |
| [placement](/cells/python-net/aspose.cells.slicers/slicer/placement) | Represents the way the drawing object is attached to the cells below it.
| [locked_aspect_ratio](/cells/python-net/aspose.cells.slicers/slicer/locked_aspect_ratio) | Indicates whether locking aspect ratio. |
| [locked_position](/cells/python-net/aspose.cells.slicers/slicer/locked_position) | Indicates whether the specified slicer can be moved or resized by using the user interface. |
| [shape](/cells/python-net/aspose.cells.slicers/slicer/shape) | Returns the Shape object associated with the specified slicer. Read-only. |
| [slicer_cache](/cells/python-net/aspose.cells.slicers/slicer/slicer_cache) | Returns the SlicerCache object associated with the slicer. Read-only. |
| [parent](/cells/python-net/aspose.cells.slicers/slicer/parent) | Returns the [`Worksheet`](/cells/python-net/aspose.cells/worksheet) object which contains this slicer. Read-only. |
| [style_type](/cells/python-net/aspose.cells.slicers/slicer/style_type) | Specify the type of Built-in slicer style
| [name](/cells/python-net/aspose.cells.slicers/slicer/name) | Returns or sets the name of the specified slicer |
| [caption](/cells/python-net/aspose.cells.slicers/slicer/caption) | Returns or sets the caption of the specified slicer. |
| [caption_visible](/cells/python-net/aspose.cells.slicers/slicer/caption_visible) | Returns or sets whether the header that displays the slicer Caption is visible
| [number_of_columns](/cells/python-net/aspose.cells.slicers/slicer/number_of_columns) | Returns or sets the number of columns in the specified slicer. |
| [left_pixel](/cells/python-net/aspose.cells.slicers/slicer/left_pixel) | Returns or sets the horizontal offset of slicer shape from its left column, in pixels. |
| [top_pixel](/cells/python-net/aspose.cells.slicers/slicer/top_pixel) | Returns or sets the vertical offset of slicer shape from its top row, in pixels. |
| [width](/cells/python-net/aspose.cells.slicers/slicer/width) | Returns or sets the width of the specified slicer, in points. |
| [width_pixel](/cells/python-net/aspose.cells.slicers/slicer/width_pixel) | Returns or sets the width of the specified slicer, in pixels. |
| [height](/cells/python-net/aspose.cells.slicers/slicer/height) | Returns or sets the height of the specified slicer, in points. |
| [height_pixel](/cells/python-net/aspose.cells.slicers/slicer/height_pixel) | Returns or sets the height of the specified slicer, in pixels. |
| [column_width_pixel](/cells/python-net/aspose.cells.slicers/slicer/column_width_pixel) | Gets or sets the width of each column in the slicer, in unit of pixels. |
| [column_width](/cells/python-net/aspose.cells.slicers/slicer/column_width) | Returns or sets the width, in points, of each column in the slicer. |
| [row_height_pixel](/cells/python-net/aspose.cells.slicers/slicer/row_height_pixel) | Returns or sets the height, in pixels, of each row in the specified slicer. |
| [row_height](/cells/python-net/aspose.cells.slicers/slicer/row_height) | Returns or sets the height, in points, of each row in the specified slicer. |
### Methods
| Method | Description |
| :- | :- |
| [`add_pivot_connection(self, pivot)`](/cells/python-net/aspose.cells.slicers/slicer/add_pivot_connection/#aspose.cells.pivot.pivottable) | Adds PivotTable connection. |
| [`remove_pivot_connection(self, pivot)`](/cells/python-net/aspose.cells.slicers/slicer/remove_pivot_connection/#aspose.cells.pivot.pivottable) | Removes PivotTable connection. |
| [`refresh(self)`](/cells/python-net/aspose.cells.slicers/slicer/refresh/#) | Refreshing the slicer.Meanwhile, Refreshing and Calculating  relative PivotTables. |
### Example
```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType
from aspose.cells.slicers import SlicerStyleType
book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
pivot.refresh_data()
pivot.calculate_data()
slicers = sheet.slicers
slicerIndex = slicers.add(pivot, "E12", "fruit")
slicer = slicers[slicerIndex]
slicer.style_type = SlicerStyleType.SLICER_STYLE_LIGHT2
items = slicer.slicer_cache.slicer_cache_items
item = items[0]
item.selected = False
# do your business
book.save("out.xlsx")
```
### See Also
* module [`aspose.cells.slicers`](..)
* class [`Worksheet`](/cells/python-net/aspose.cells/worksheet)
