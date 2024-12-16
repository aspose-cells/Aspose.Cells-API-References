---
title: Aspose::Cells::AbstractFormulaChangeMonitor class
linktitle: AbstractFormulaChangeMonitor
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::AbstractFormulaChangeMonitor class. Monitor for user to track the change of formulas during certain operations in C++.'
type: docs
weight: 300
url: /cpp/aspose.cells/abstractformulachangemonitor/
---
## AbstractFormulaChangeMonitor class


Monitor for user to track the change of formulas during certain operations.

```cpp
class AbstractFormulaChangeMonitor
```

## Methods

| Method | Description |
| --- | --- |
| [AbstractFormulaChangeMonitor(AbstractFormulaChangeMonitor_Impl* impl)](./abstractformulachangemonitor/) | Constructs from an implementation object. |
| [AbstractFormulaChangeMonitor(const AbstractFormulaChangeMonitor\& src)](./abstractformulachangemonitor/) | Copy constructor. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [OnCellFormulaChanged(int32_t sheetIndex, int32_t rowIndex, int32_t columnIndex)](./oncellformulachanged/) | The event that will be triggered when the formula in a cell is changed. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const AbstractFormulaChangeMonitor\& src)](./operator_asm/) | operator= |
| [~AbstractFormulaChangeMonitor()](./~abstractformulachangemonitor/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks


For example, while deleting/inserting range of cells, formulas of other cells may be changed because of the shift of references.
## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
