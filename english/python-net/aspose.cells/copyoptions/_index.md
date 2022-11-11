---
title: CopyOptions
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 360
url: /cells/python-net/aspose.cells/copyoptions/
---

## CopyOptions class

Represents the copy options.

The CopyOptions type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|CopyOptions()|CopyOptions constructor.|
## Properties
| Name | Description |
| :- | :- |
|keep_macros|Indicates whether keeping macros;|
|extend_to_adjacent_range|Indicates whether extend ranges when copying the range to adjacent range.|
|copy_names|Indicates whether copying the names.|
|copy_invalid_formulas_as_values|If the formula is not valid for the dest destination, only copy values.|
|column_character_width|Indicates whether copying column width in unit of characters.|
|refer_to_sheet_with_same_name|When copying a worksheet to another workbook and the worksheet contains the formulas which refer to other worksheets in MS Excel,<br/>            the copied formulas should refer to source workbook. <br/>            But sometimes we have copied other worksheets and we hope the copied formulas refer to other worksheets with the name in the same workbook,<br/>            please set this property as true.|
|refer_to_destination_sheet|When copying the range in the same file and the chart refers to the source sheet,<br/>            False means the copied chart's data source will not be changed.<br/>            True means the copied chart's data source refers to the destination sheet.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

