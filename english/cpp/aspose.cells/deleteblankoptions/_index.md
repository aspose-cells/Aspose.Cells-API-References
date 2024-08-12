---
title: Aspose::Cells::DeleteBlankOptions class
linktitle: DeleteBlankOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::DeleteBlankOptions class. Represents the setting of deleting blank cells/rows/columns in C++.'
type: docs
weight: 4600
url: /cpp/aspose.cells/deleteblankoptions/
---
## DeleteBlankOptions class


Represents the setting of deleting blank cells/rows/columns.

```cpp
class DeleteBlankOptions : public Aspose::Cells::DeleteOptions
```

## Methods

| Method | Description |
| --- | --- |
| [DeleteBlankOptions()](./deleteblankoptions/) | Default constructor. |
| [DeleteBlankOptions(DeleteBlankOptions_Impl* impl)](./deleteblankoptions/) | Constructs from an implementation object. |
| [DeleteBlankOptions(const DeleteBlankOptions\& src)](./deleteblankoptions/) | Copy constructor. |
| [DeleteBlankOptions(const DeleteOptions\& src)](./deleteblankoptions/) | Constructs from a parent object. |
| [DeleteOptions()](../deleteoptions/deleteoptions/) | Default constructor. |
| [DeleteOptions(DeleteOptions_Impl* impl)](../deleteoptions/deleteoptions/) | Constructs from an implementation object. |
| [DeleteOptions(const DeleteOptions\& src)](../deleteoptions/deleteoptions/) | Copy constructor. |
| [GetEmptyFormulaValueAsBlank()](./getemptyformulavalueasblank/) | Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false. |
| [GetEmptyStringAsBlank()](./getemptystringasblank/) | Whether one cell will be taken as blank when its value is empty string. Default value is true. |
| [GetMergedCellsShrinkType()](./getmergedcellsshrinktype/) | Indicates how to process merged cells when deleting blank rows/columns.<br>  For [MergedCellsShrinkType.KeepHeaderOnly](../mergedcellsshrinktype/), all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property.<br>  For [MergedCellsShrinkType.None](../mergedcellsshrinktype/), all cells in it will be taken as non-blank.<br>  For [MergedCellsShrinkType.ShrinkToFit](../mergedcellsshrinktype/), all cells outside the content display area will be taken as blank.<br> |
| [GetUpdateReference()](../deleteoptions/getupdatereference/) | Indicates if update references in other worksheets. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const DeleteBlankOptions\& src)](./operator_asm/) | operator= |
| [operator=(const DeleteOptions\& src)](../deleteoptions/operator_asm/) | operator= |
| [SetEmptyFormulaValueAsBlank(bool value)](./setemptyformulavalueasblank/) | Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false. |
| [SetEmptyStringAsBlank(bool value)](./setemptystringasblank/) | Whether one cell will be taken as blank when its value is empty string. Default value is true. |
| [SetMergedCellsShrinkType(MergedCellsShrinkType value)](./setmergedcellsshrinktype/) | Indicates how to process merged cells when deleting blank rows/columns.<br>  For [MergedCellsShrinkType.KeepHeaderOnly](../mergedcellsshrinktype/), all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property.<br>  For [MergedCellsShrinkType.None](../mergedcellsshrinktype/), all cells in it will be taken as non-blank.<br>  For [MergedCellsShrinkType.ShrinkToFit](../mergedcellsshrinktype/), all cells outside the content display area will be taken as blank.<br> |
| [SetUpdateReference(bool value)](../deleteoptions/setupdatereference/) | Indicates if update references in other worksheets. |
| [~DeleteBlankOptions()](./~deleteblankoptions/) | Destructor. |
| [~DeleteOptions()](../deleteoptions/~deleteoptions/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Class [DeleteOptions](../deleteoptions/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
