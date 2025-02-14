﻿---
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
| virtual [OnCellFormulaChanged(int32_t sheetIndex, int32_t rowIndex, int32_t columnIndex)](./oncellformulachanged/) | The event that will be triggered when the formula in a cell is changed. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks


For example, while deleting/inserting range of cells, formulas of other cells may be changed because of the shift of references.

## Examples


```cpp
Aspose::Cells::Startup();
class MyFormulaChangeMonitor : public AbstractFormulaChangeMonitor
{
private:
    WorksheetCollection* mWorksheets;
public:
    MyFormulaChangeMonitor(WorksheetCollection& worksheets)
    {
        mWorksheets = &worksheets;
    }

    void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
    {
        int i = rowIndex;
        std::cout << "Cell " << mWorksheets->Get(sheetIndex).GetName().ToUtf8() << "!"
            << CellsHelper::CellIndexToName(rowIndex, columnIndex).ToUtf8()
            << "'s formula was changed while inserting rows." << std::endl;
    }
};

   Workbook wb(u"template.xlsx");
WorksheetCollection wc = wb.GetWorksheets();
MyFormulaChangeMonitor my(wc);
InsertOptions options;
options.SetFormulaChangeMonitor(&my);
wb.GetWorksheets().Get(0).GetCells().InsertRows(0, 2, options);
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
