---
title: Class AbstractFormulaChangeMonitor
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.AbstractFormulaChangeMonitor class. Monitor for user to track the change of formulas during certain operations
type: docs
url: /net/aspose.cells/abstractformulachangemonitor/
---
## AbstractFormulaChangeMonitor class

Monitor for user to track the change of formulas during certain operations.

```csharp
public abstract class AbstractFormulaChangeMonitor
```

## Methods

| Name | Description |
| --- | --- |
| virtual [OnCellFormulaChanged](../../aspose.cells/abstractformulachangemonitor/oncellformulachanged/)(int, int, int) | The event that will be triggered when the formula in a cell is changed. |

### Remarks

For example, while deleting/inserting range of cells, formulas of other cells may be changed because of the shift of references.

### Examples

```csharp
[C#]
Workbook wb = new Workbook("template.xlsx");
InsertOptions options = new InsertOptions();
options.CellChangeMonitor = new MyFormulaChangeMonitor(wb.Worksheets);
wb.Worksheets[0].Cells.InsertRows(0, 2, options);

class MyFormulaChangeMonitor : AbstractFormulaChangeMonitor
{
    private readonly WorksheetCollection mWorksheets;
    public MyFormulaChangeMonitor(WorksheetCollection worksheets)
    {
        mWorksheets = worksheet;
    }
    public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
    {
        Console.WriteLine("Cell " + mWorksheets[sheetIndex].Name + "!"
            + CellsHelper.CellIndexToName(rowIndex, columnIndex)
            + "'s formula was changed while inserting rows.");
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


