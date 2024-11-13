---
title: DeleteBlankOptions.MergedCellsShrinkType
second_title: Aspose.Cells for .NET API Reference
description: DeleteBlankOptions property. Indicates how to process merged cells when deleting blank rows/columns
type: docs
url: /net/aspose.cells/deleteblankoptions/mergedcellsshrinktype/
---
## DeleteBlankOptions.MergedCellsShrinkType property

Indicates how to process merged cells when deleting blank rows/columns.

```csharp
public MergedCellsShrinkType MergedCellsShrinkType { get; set; }
```

### Remarks

For KeepHeaderOnly, all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property. For None, all cells in it will be taken as non-blank. For ShrinkToFit, all cells outside the content display area will be taken as blank.

### See Also

* enum [MergedCellsShrinkType](../../mergedcellsshrinktype/)
* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


