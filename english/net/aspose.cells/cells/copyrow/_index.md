---
title: Cells.CopyRow
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Copies data and formats of a whole row
type: docs
url: /net/aspose.cells/cells/copyrow/
---
## Cells.CopyRow method

Copies data and formats of a whole row.

```csharp
public void CopyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |

### Examples

```csharp
// Called: cells.CopyRow(cells2, cells2.Rows[row].Index, cells.Rows[row - 1].Index);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CopyRow_119419.xls");

            Worksheet worksheet1 = workbook.Worksheets[0];
            Worksheet worksheet2 = workbook.Worksheets[1];
            Cells cells = worksheet1.Cells;
            Cells cells2 = worksheet2.Cells;

            int row = 15;

            // CopyRow from 'Sheet2' to 'Sheet1'
            cells.CopyRow(cells2, cells2.Rows[row].Index, cells.Rows[row - 2].Index);
            cells.CopyRow(cells2, cells2.Rows[row].Index, cells.Rows[row - 1].Index);
            cells.CopyRow(cells2, cells2.Rows[row].Index, cells.Rows[row].Index);
            cells.CopyRow(cells2, cells2.Rows[row].Index, cells.Rows[row + 1].Index);

            // CopyRow in 'Sheet2'
            cells2.CopyRow(cells2, cells2.Rows[row].Index, cells2.Rows[row - 2].Index);
            cells2.CopyRow(cells2, cells2.Rows[row].Index, cells2.Rows[row - 1].Index);
            cells2.CopyRow(cells2, cells2.Rows[row].Index, cells2.Rows[row + 1].Index);

            Assert.AreEqual(cells["C14"].StringValue,"aaaa");
            Assert.AreEqual(cells2["C14"].StringValue, "aaaa");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


