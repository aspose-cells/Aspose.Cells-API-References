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
            sheet.Cells[0, 0].Value = &quot;Col A&quot;; sheet.Cells[0, 1].Value = &quot;Col B&quot;; sheet.Cells[0, 2].Value = &quot;Col C&quot;;
            sheet.Cells[1, 0].Value = &quot;A1&quot;; sheet.Cells[1, 1].Value = &quot;B1&quot;; sheet.Cells[1, 2].Value = &quot;C1&quot;;
            sheet.Cells[2, 0].Value = &quot;A2&quot;; sheet.Cells[2, 1].Value = &quot;B2&quot;; sheet.Cells[2, 2].Value = &quot;C2&quot;;
            sheet.Cells[3, 0].Value = &quot;A1&quot;; sheet.Cells[3, 1].Value = &quot;B1&quot;; sheet.Cells[3, 2].Value = &quot;C1&quot;;
            sheet.Cells[4, 0].Value = &quot;A3&quot;; sheet.Cells[4, 1].Value = &quot;B3&quot;; sheet.Cells[4, 2].Value = &quot;C3&quot;;
            var columnOffsets = new int[] { 1, 2 };
            sheet.Cells.RemoveDuplicates(sheet.Cells.MinDataRow, sheet.Cells.MinDataColumn, sheet.Cells.MaxDataRow, sheet.Cells.MaxDataColumn, true, columnOffsets);
            Assert.AreEqual(&quot;B3&quot;, sheet.Cells[&quot;B4&quot;].StringValue);
            workbook.Save(Constants.destPath + &quot;CellsNet47250.xlsx&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


