##Aspose::Cells::DeleteBlankOptions::GetMergedCellsShrinkType method
'Aspose::Cells::DeleteBlankOptions::GetMergedCellsShrinkType method. Indicates how to process merged cells when deleting blank rows/columns in C++.'
## DeleteBlankOptions::GetMergedCellsShrinkType method
Indicates how to process merged cells when deleting blank rows/columns.
```cpp
MergedCellsShrinkType Aspose::Cells::DeleteBlankOptions::GetMergedCellsShrinkType()
```
## Remarks
For [MergedCellsShrinkType.KeepHeaderOnly](../../mergedcellsshrinktype/), all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property.
For [MergedCellsShrinkType.None](../../mergedcellsshrinktype/), all cells in it will be taken as non-blank.
For [MergedCellsShrinkType.ShrinkToFit](../../mergedcellsshrinktype/), all cells outside the content display area will be taken as blank.
## See Also
* Enum [MergedCellsShrinkType](../../mergedcellsshrinktype/)
* Class [DeleteBlankOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
