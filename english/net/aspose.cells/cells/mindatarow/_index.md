---
title: Cells.MinDataRow
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Minimum row index of cell which contains data
type: docs
url: /net/aspose.cells/cells/mindatarow/
---
## Cells.MinDataRow property

Minimum row index of cell which contains data.

```csharp
public int MinDataRow { get; }
```

### Remarks

Return -1 if there is no cell which contains data.

### Examples

```csharp
// Called: sheet.Cells.RemoveDuplicates(sheet.Cells.MinDataRow, sheet.Cells.MinDataColumn, sheet.Cells.MaxDataRow, sheet.Cells.MaxDataColumn, true, columnOffsets);
[Test]
        public void Property_MinDataRow()
        {
            var workbook = new Workbook();
            var sheet = workbook.Worksheets[0];
            sheet.Cells[0, 0].Value = "Col A"; sheet.Cells[0, 1].Value = "Col B"; sheet.Cells[0, 2].Value = "Col C";
            sheet.Cells[1, 0].Value = "A1"; sheet.Cells[1, 1].Value = "B1"; sheet.Cells[1, 2].Value = "C1";
            sheet.Cells[2, 0].Value = "A2"; sheet.Cells[2, 1].Value = "B2"; sheet.Cells[2, 2].Value = "C2";
            sheet.Cells[3, 0].Value = "A1"; sheet.Cells[3, 1].Value = "B1"; sheet.Cells[3, 2].Value = "C1";
            sheet.Cells[4, 0].Value = "A3"; sheet.Cells[4, 1].Value = "B3"; sheet.Cells[4, 2].Value = "C3";
            var columnOffsets = new int[] { 1, 2 };
            sheet.Cells.RemoveDuplicates(sheet.Cells.MinDataRow, sheet.Cells.MinDataColumn, sheet.Cells.MaxDataRow, sheet.Cells.MaxDataColumn, true, columnOffsets);
            Assert.AreEqual("B3", sheet.Cells["B4"].StringValue);
            workbook.Save(Constants.destPath + "CellsNet47250.xlsx");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


