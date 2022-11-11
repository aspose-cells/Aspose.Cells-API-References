---
title: AccessCacheOptions
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 4270
url: /python-net/aspose.cells/accesscacheoptions/
---

## AccessCacheOptions enumeration

Cache options for data access. Can be combined with | operator for multiple options together.

## Members
| Member name | Description |
| :- | :- |
|NONE|No cache for any data access.|
|ALL|Apply all possible optimizations for all kinds of data access in the workbook.<br/>            All settings and data should not be changed during the optimized access.|
|POSITION_AND_SIZE|Apply possible optimization for getting object(such as Shape)'s position and size.<br/>            Row height and column width settings should not be changed during the optimized access.|
|CELLS_DATA|Apply possible optimization for getting cells' values.<br/>            Cells data(data and settings of Cell, Row) should not be changed during<br/>            the optimized access, no new Cell/Row objects should be created either(such as<br/>            by|
|CELL_DISPLAY|Apply possible optimization for getting display-related results of<br/>            cells([display_string_value](/python-net/aspose.cells/cell/), [None](/python-net/aspose.cells/cell/), [None](/python-net/aspose.cells/cell/), etc.).<br/>            Cells data and style-related objects(Cell/Row/Column styles, column width, etc.) should not be changed<br/>            during the optimized access.|
|GET_FORMULA|Apply possible optimization for getting formulas.<br/>            All data and settings which may affect the formula expression(Worksheet's name, Name's text,<br/>            table's column, etc.) should not be changed during the optimized access.|
|SET_FORMULA|Apply possible optimization for setting formulas.<br/>            All data and settings which may affect the formula expression(Worksheet's name, Name's text,<br/>            table's column, etc.) should not be changed during the optimized access.|
|CALCULATE_FORMULA|Apply possible optimization for calculating formulas.<br/>            Cells data should not be changed during the optimized access, none new objects(Cell, Row, etc.)<br/>            should be created either(such as by|
|CONDITIONAL_FORMATTING|Apply possible optimization for getting formatting result of conditional formattings.<br/>            All data and settings which may affect the result of conditional formattings(settings of<br/>            conditional formattings, dependent cell values, etc.) should not be changed during the optimized access.|
|VALIDATION|Apply possible optimization for getting validation result.<br/>            All data and settings which may affect the result of validation(settings of the validation,<br/>            dependent cell values, etc.) should not be changed during the optimized access.|

### See Also

* namespace [aspose.cells](/python-net/aspose.cells/)
* assembly [Aspose.Cells](/python-net/)

