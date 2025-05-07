---
title: Cells.CopyColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Copies data and formats of a whole column
type: docs
url: /net/aspose.cells/cells/copycolumn/
---
## Cells.CopyColumn method

Copies data and formats of a whole column.

```csharp
public void CopyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Int32 | Source column index. |
| destinationColumnIndex | Int32 | Destination column index. |

### Examples

```csharp
// Called: cells.CopyColumn(cells, 0, 11);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsNet53408.xlsx");
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
          //  Console.WriteLine("A1: " + cells["A1"].StringValue + "  B1: " + cells["B1"].StringValue + " C1: " + cells["C1"].StringValue);
            cells.CopyColumn(cells, 0, 1);
            // Console.WriteLine("A1: " + cells["A1"].StringValue + "  B1: " + cells["B1"].StringValue + " C1: " + cells["C1"].StringValue);
       
            cells.CopyColumn(cells, 0, 4);
            cells.CopyColumn(cells, 0, 11);
            cells.CopyColumn(cells, 0, 18);
            Assert.AreEqual("", cells["B1"].StringValue);
            Assert.AreEqual("Merged Source", cells["E1"].StringValue);
            Assert.AreEqual("Merged Source", cells["L1"].StringValue);
            Assert.AreEqual("", cells["R1"].StringValue);
            wb.Save(Constants.destPath + "CellsNet53408.xlsx");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


