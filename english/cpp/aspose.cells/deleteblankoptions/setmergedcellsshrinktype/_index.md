---
title: Aspose::Cells::DeleteBlankOptions::SetMergedCellsShrinkType method
linktitle: SetMergedCellsShrinkType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::DeleteBlankOptions::SetMergedCellsShrinkType method. Indicates how to process merged cells when deleting blank rows/columns in C++.'
type: docs
weight: 1300
url: /cpp/aspose.cells/deleteblankoptions/setmergedcellsshrinktype/
---
## DeleteBlankOptions::SetMergedCellsShrinkType method


Indicates how to process merged cells when deleting blank rows/columns.

```cpp
void Aspose::Cells::DeleteBlankOptions::SetMergedCellsShrinkType(MergedCellsShrinkType value)
```

## Remarks


For [MergedCellsShrinkType.KeepHeaderOnly](../../mergedcellsshrinktype/), all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property.

 For [MergedCellsShrinkType.None](../../mergedcellsshrinktype/), all cells in it will be taken as non-blank.

 For [MergedCellsShrinkType.ShrinkToFit](../../mergedcellsshrinktype/), all cells outside the content display area will be taken as blank.

## See Also

* Class [Vector](../../vector/)
* Enum [MergedCellsShrinkType](../../mergedcellsshrinktype/)
* Class [DeleteBlankOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
