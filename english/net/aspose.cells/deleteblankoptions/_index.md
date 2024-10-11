---
title: Class DeleteBlankOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.DeleteBlankOptions class. Represents the setting of deleting blank cells/rows/columns
type: docs
url: /net/aspose.cells/deleteblankoptions/
---
## DeleteBlankOptions class

Represents the setting of deleting blank cells/rows/columns.

```csharp
public class DeleteBlankOptions : DeleteOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [DeleteBlankOptions](deleteblankoptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [DrawingsAsBlank](../../aspose.cells/deleteblankoptions/drawingsasblank/) { get; set; } | Whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true. |
| [EmptyFormulaValueAsBlank](../../aspose.cells/deleteblankoptions/emptyformulavalueasblank/) { get; set; } | Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false. |
| [EmptyStringAsBlank](../../aspose.cells/deleteblankoptions/emptystringasblank/) { get; set; } | Whether one cell will be taken as blank when its value is empty string. Default value is true. |
| [EndIndex](../../aspose.cells/deleteblankoptions/endindex/) { get; set; } | Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked. |
| [MergedCellsShrinkType](../../aspose.cells/deleteblankoptions/mergedcellsshrinktype/) { get; set; } | Indicates how to process merged cells when deleting blank rows/columns. For KeepHeaderOnly, all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property. For None, all cells in it will be taken as non-blank. For ShrinkToFit, all cells outside the content display area will be taken as blank. |
| [StartIndex](../../aspose.cells/deleteblankoptions/startindex/) { get; set; } | Specifies the start row/column index of the range to check and delete blank rows/columns. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Indicates if update references in other worksheets.(Inherited from [`DeleteOptions`](../deleteoptions/).) |

### See Also

* class [DeleteOptions](../deleteoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


