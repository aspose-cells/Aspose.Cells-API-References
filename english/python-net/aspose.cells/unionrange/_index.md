---
title: UnionRange
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 1520
url: /python-net/aspose.cells/unionrange/
---

## UnionRange class

Represents union range.

The UnionRange type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|first_row|Gets the index of the first row of the range.|
|first_column|Gets the index of the first column of the range.|
|row_count|Gets the count of rows in the range.|
|column_count|Gets the count of rows in the range.|
|value|Gets and sets the values of the range.|
|name|Gets or sets the name of the range.|
|refers_to|Gets the range's refers to.|
|has_range|Indicates whether this has range.|
|hyperlinks|Gets all hyperlink in the range.|
|cell_count|Gets all cell count in the range.|
|range_count|Gets the count of the ranges.|
|ranges|Gets all union ranges.|
## Methods
| Name | Description |
| :- | :- |
|set_outline_borders(border_styles, border_colors)|Sets out line borders around a range of cells.|
|set_outline_borders(border_style, border_color)|Sets out line borders around a range of cells.|
|intersect(range)|Intersects another range.|
|intersect(union_range)|Intersects another range.|
|intersect(ranges)|Intersects another range.|
|union(range)|Union another range.|
|union(union_range)|Union another range.|
|union(ranges)|Union the ranges.|
|merge()|Combines a range of cells into a single cell.|
|un_merge()|Unmerges merged cells of this range.|
|put_value(string_value, is_converted, set_style)|Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset.|
|set_style(style)|Sets the style of the range.|
|apply_style(style, flag)|Applies formats for a whole range.|
|copy(range, options)|Copying the range with paste special options.|
|get_enumerator()|Gets the enumerator for cells in this Range.|

### See Also

* namespace [aspose.cells](/python-net/aspose.cells/)
* assembly [Aspose.Cells](/python-net/)

