---
title: Name
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 1070
url: /cells/python-net/aspose.cells/name/
---

## Name class

Represents a defined name for a range of cells.

The Name type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|comment|Gets and sets the comment of the name.<br/>            Only applies for Excel 2007.|
|text|Gets the name text of the object.|
|full_text|Gets the name  full text of the object with the scope setting.|
|refers_to|Returns or sets the formula that the name is defined to refer to, beginning with an equal sign.|
|r1c1_refers_to|Gets or sets a R1C1 reference of the [Name](/cells/python-net/aspose.cells/name/).|
|is_referred|Indicates whether this name is referred by other formulas.|
|is_visible|Indicates whether the name is visible.|
|sheet_index|Indicates this name belongs to Workbook or Worksheet.<br/>            0 = Global name, otherwise index to sheet (one-based)|
## Methods
| Name | Description |
| :- | :- |
|get_refers_to(is_r1c1, is_local)|Get the reference of this Name.|
|get_refers_to(is_r1c1, is_local, row, column)|Get the reference of this Name based on specified cell.|
|get_ranges()|Gets all ranges referred by this name.|
|get_ranges(recalculate)|Gets all ranges referred by this name.|
|get_range()|Gets all ranges referred by this name.|
|get_range(recalculate)|Gets all ranges referred by this name.|
|get_range(sheet_index, row, column)|Gets the range if this name refers to a range.<br/>            If the reference of this name is not absolute, the range may be different for different cell.|
|set_refers_to(refers_to, is_r1c1, is_local)|Set the reference of this Name.|
|get_referred_areas(recalculate)|Gets all references referred by this name.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

