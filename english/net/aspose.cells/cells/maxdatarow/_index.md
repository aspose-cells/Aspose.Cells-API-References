---
title: Cells.MaxDataRow
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Maximum row index of cell which contains data
type: docs
url: /net/aspose.cells/cells/maxdatarow/
---
## Cells.MaxDataRow property

Maximum row index of cell which contains data.

```csharp
public int MaxDataRow { get; }
```

### Remarks

Return -1 if there is no cell which contains data.

### Examples

```csharp
// Called: CellArea ca = new CellArea() { StartRow = 4, StartColumn = 0, EndRow = sheet.Cells.MaxDataRow, EndColumn = sheet.Cells.MaxDataColumn };
public void Cells_Property_MaxDataRow()
{
    Workbook wb = new Workbook(Constants.sourcePath + "TestSubT.xls");
    Worksheet sheet = wb.Worksheets[0];
    CellArea ca = new CellArea() { StartRow = 4, StartColumn = 0, EndRow = sheet.Cells.MaxDataRow, EndColumn = sheet.Cells.MaxDataColumn };
    sheet.Cells.Subtotal(ca, 0, ConsolidationFunction.CountNums, new int[] { 1 }, false, false, true);
    ca = new CellArea() { StartRow = 4, StartColumn = 0, EndRow = sheet.Cells.MaxDataRow, EndColumn = sheet.Cells.MaxDataColumn };
    sheet.Cells.Subtotal(ca, 0, ConsolidationFunction.Max, new int[] { 1 }, false, false, true);
    Assert.AreEqual(sheet.Cells["B24"].GetStyle().Custom, "m/d/yyyy\\ h:mm\\ AM/PM");
    wb.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


