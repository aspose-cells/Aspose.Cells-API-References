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
// Called: Assert.AreEqual("#N/A", cell.StringValue);
[Test]
        public void Property_StringValue()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue(3);
            cells[1, 0].PutValue(3);
            cells[2, 0].PutValue(2);
            cells[3, 0].PutValue(6);
            cells[4, 0].PutValue(5);
            Cell cell = cells[0, 1];
            cell.Formula = "=MATCH(7,A1:A5,0)";
            workbook.CalculateFormula();
            Assert.AreEqual("#N/A", cell.StringValue);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


