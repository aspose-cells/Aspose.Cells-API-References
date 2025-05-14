---
title: Cell.Calculate
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Calculates the formula of the cell
type: docs
url: /net/aspose.cells/cell/calculate/
---
## Cell.Calculate method

Calculates the formula of the cell.

```csharp
public void Calculate(CalculationOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options for calculation |

### Examples

```csharp
// Called: cell.Calculate(new CalculationOptions());
public void Cell_Method_Calculate()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    CellArea ca = CellArea.CreateCellArea(0, 0, 2, 2);
    Process(sheet, "=IF({2;1;3}>1,{1;2},{4,8,16})", ca,
        new string[] { "1", "1", "1", "4", "8", "16", "#N/A", "#N/A", "#N/A", });
    Process(sheet, "=IF({2;1;1}>1,{1;2},{4,8,16})", ca,
        new string[] { "1", "1", "1", "4", "8", "16", "4", "8", "16", });
    Process(sheet, "=IF({1;2;3}>1,MATCH({1,2,3},{1,2,3},0),0)", ca,
        new string[] { "0", "0", "0", "1", "2", "3", "1", "2", "3", });
    Cell cell = sheet.Cells[0, 0];
    cell.Formula = "=SUM(IF({1;2;3}>1,MATCH({1,2,3},{1,2,3},0),0))";
    cell.Calculate(new CalculationOptions());
    Assert.AreEqual(12, cell.IntValue);
    cell.SetArrayFormula("=SUM(IF({1;2;3}>1,MATCH({1,2,3},{1,2,3},0),0))", 1, 1);
    cell.Calculate(new CalculationOptions());
    Assert.AreEqual(12, cell.IntValue);
}
```

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


