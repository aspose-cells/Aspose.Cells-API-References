##UnionRange class
## UnionRange class
Represents union range.
The UnionRange type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [first_row](/cells/python-net/aspose.cells/unionrange/first_row) | Gets the index of the first row of the range. |
| [first_column](/cells/python-net/aspose.cells/unionrange/first_column) | Gets the index of the first column of the range. |
| [row_count](/cells/python-net/aspose.cells/unionrange/row_count) | Gets the count of rows in the range. |
| [column_count](/cells/python-net/aspose.cells/unionrange/column_count) | Gets the count of rows in the range. |
| [value](/cells/python-net/aspose.cells/unionrange/value) | Gets and sets the values of the range. |
| [name](/cells/python-net/aspose.cells/unionrange/name) | Gets or sets the name of the range. |
| [refers_to](/cells/python-net/aspose.cells/unionrange/refers_to) | Gets the range's refers to. |
| [has_range](/cells/python-net/aspose.cells/unionrange/has_range) | Indicates whether this has range. |
| [hyperlinks](/cells/python-net/aspose.cells/unionrange/hyperlinks) | Gets all hyperlink in the range. |
| [cell_count](/cells/python-net/aspose.cells/unionrange/cell_count) | Gets all cell count in the range. |
| [range_count](/cells/python-net/aspose.cells/unionrange/range_count) | Gets the count of the ranges. |
| [ranges](/cells/python-net/aspose.cells/unionrange/ranges) | Gets all union ranges. |
### Methods
| Method | Description |
| :- | :- |
| [`set_outline_borders(self, border_styles, border_colors)`](/cells/python-net/aspose.cells/unionrange/set_outline_borders/#list-aspose.pydrawing.color[]) | Sets out line borders around a range of cells. |
| [`set_outline_borders(self, border_style, border_color)`](/cells/python-net/aspose.cells/unionrange/set_outline_borders/#aspose.cells.cellbordertype-aspose.pydrawing.color) | Sets the outline borders around a range of cells with same border style and color. |
| [`intersect(self, range)`](/cells/python-net/aspose.cells/unionrange/intersect/#system.string) | Intersects another range. |
| [`intersect(self, union_range)`](/cells/python-net/aspose.cells/unionrange/intersect/#aspose.cells.unionrange) | Intersects another range. |
| [`intersect(self, ranges)`](/cells/python-net/aspose.cells/unionrange/intersect/#list) | Intersects another range. |
| [`union(self, range)`](/cells/python-net/aspose.cells/unionrange/union/#system.string) | Union another range. |
| [`union(self, union_range)`](/cells/python-net/aspose.cells/unionrange/union/#aspose.cells.unionrange) | Union another range. |
| [`union(self, ranges)`](/cells/python-net/aspose.cells/unionrange/union/#list) | Union the ranges. |
| [`merge(self)`](/cells/python-net/aspose.cells/unionrange/merge/#) | Combines a range of cells into a single cell. |
| [`un_merge(self)`](/cells/python-net/aspose.cells/unionrange/un_merge/#) | Unmerges merged cells of this range. |
| [`put_value(self, string_value, is_converted, set_style)`](/cells/python-net/aspose.cells/unionrange/put_value/#system.string-bool-bool) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [`set_style(self, style)`](/cells/python-net/aspose.cells/unionrange/set_style/#aspose.cells.style) | Sets the style of the range. |
| [`apply_style(self, style, flag)`](/cells/python-net/aspose.cells/unionrange/apply_style/#aspose.cells.style-aspose.cells.styleflag) | Applies formats for a whole range. |
| [`copy(self, range, options)`](/cells/python-net/aspose.cells/unionrange/copy/#aspose.cells.unionrange-aspose.cells.pasteoptions) | Copying the range with paste special options. |
### See Also
* module [`aspose.cells`](..)
