---
title: Aspose::Cells::DeleteBlankOptions class
linktitle: DeleteBlankOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::DeleteBlankOptions class. Represents the setting of deleting blank cells/rows/columns in C++.'
type: docs
weight: 4800
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
| [GetDrawingsAsBlank()](./getdrawingsasblank/) | Indicates whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true. |
| [GetEmptyFormulaValueAsBlank()](./getemptyformulavalueasblank/) | Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string. Default value is false. |
| [GetEmptyStringAsBlank()](./getemptystringasblank/) | Indicates whether one cell will be taken as blank when its value is an empty string. Default value is true. |
| [GetEndIndex()](./getendindex/) | Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked. |
| [GetFormulaChangeMonitor()](../deleteoptions/getformulachangemonitor/) | Gets/sets the monitor for tracking changes caused by the deletion. |
| [GetMergedCellsShrinkType()](./getmergedcellsshrinktype/) | Indicates how to process merged cells when deleting blank rows/columns. |
| [GetStartIndex()](./getstartindex/) | Specifies the start row/column index of the range to check and delete blank row/column. |
| [GetUpdateReference()](../deleteoptions/getupdatereference/) | Indicates if update references in other worksheets. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const DeleteBlankOptions\& src)](./operator_asm/) | operator= |
| [operator=(const DeleteOptions\& src)](../deleteoptions/operator_asm/) | operator= |
| [SetDrawingsAsBlank(bool value)](./setdrawingsasblank/) | Indicates whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true. |
| [SetEmptyFormulaValueAsBlank(bool value)](./setemptyformulavalueasblank/) | Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string. Default value is false. |
| [SetEmptyStringAsBlank(bool value)](./setemptystringasblank/) | Indicates whether one cell will be taken as blank when its value is an empty string. Default value is true. |
| [SetEndIndex(int32_t value)](./setendindex/) | Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked. |
| [SetFormulaChangeMonitor(AbstractFormulaChangeMonitor* value)](../deleteoptions/setformulachangemonitor/) | Gets/sets the monitor for tracking changes caused by the deletion. |
| [SetMergedCellsShrinkType(MergedCellsShrinkType value)](./setmergedcellsshrinktype/) | Indicates how to process merged cells when deleting blank rows/columns. |
| [SetStartIndex(int32_t value)](./setstartindex/) | Specifies the start row/column index of the range to check and delete blank row/column. |
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
