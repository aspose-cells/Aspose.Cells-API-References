---
title: Cell.StringValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the string value contained in the cell. If the type of this cell is string then return the string value itself. For other cell types the formatted string value formatted with the specified style of this cell will be returned. The formatted cell value is same with what you can get from excel when copying a cell as textsuch as copying cell to text editor or exporting to csv
type: docs
url: /net/aspose.cells/cell/stringvalue/
---
## Cell.StringValue property

Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself. For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned. The formatted cell value is same with what you can get from excel when copying a cell as text(such as copying cell to text editor or exporting to csv).

```csharp
public string StringValue { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("#REF!", cell.StringValue);
public void Cell_Property_StringValue()
{
  Workbook workbook = new Workbook();
  Cells cells = workbook.Worksheets[0].Cells;
  cells[1, 2].PutValue(1);
  cells[2, 2].PutValue(2);
  cells[3, 2].PutValue(3);
  cells[1, 3].PutValue(4);
  cells[2, 3].PutValue(5);
  cells[3, 3].PutValue(6);
  cells[1, 4].PutValue(7);
  cells[2, 4].PutValue(8);
  cells[3, 4].PutValue(9);
  Cell cell = cells[0, 0];
  cell.Formula = "=SUM(OFFSET(C3:E5,-1,0,0,0))";
  workbook.CalculateFormula();
  Assert.AreEqual("#REF!", cell.StringValue);
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


