---
title: Row.Index
second_title: Aspose.Cells for .NET API Reference
description: Row property. Gets the index of this row
type: docs
url: /net/aspose.cells/row/index/
---
## Row.Index property

Gets the index of this row.

```csharp
public int Index { get; }
```

### Examples

```csharp
// Called: cells.CopyRow(cells2, cells2.Rows[row].Index, cells.Rows[row - 1].Index);
[Test]
        public void Property_Index()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CopyRow_119419.xls&quot;);

            Worksheet worksheet1 = workbook.Worksheets[0];
            Worksheet worksheet2 = workbook.Worksheets[1];
            Cells cells = worksheet1.Cells;
            Cells cells2 = worksheet2.Cells;

            int row = 15;

            // CopyRow from &apos;Sheet2&apos; to &apos;Sheet1&apos;
            cells.CopyRow(cells2, cells2.Rows[row].Index, cells.Rows[row - 2].Index);
            cells.CopyRow(cells2, cells2.Rows[row].Index, cells.Rows[row - 1].Index);
            cells.CopyRow(cells2, cells2.Rows[row].Index, cells.Rows[row].Index);
            cells.CopyRow(cells2, cells2.Rows[row].Index, cells.Rows[row + 1].Index);

            // CopyRow in &apos;Sheet2&apos;
            cells2.CopyRow(cells2, cells2.Rows[row].Index, cells2.Rows[row - 2].Index);
            cells2.CopyRow(cells2, cells2.Rows[row].Index, cells2.Rows[row - 1].Index);
            cells2.CopyRow(cells2, cells2.Rows[row].Index, cells2.Rows[row + 1].Index);

            Assert.AreEqual(cells[&quot;C14&quot;].StringValue,&quot;aaaa&quot;);
            Assert.AreEqual(cells2[&quot;C14&quot;].StringValue, &quot;aaaa&quot;);
        }
```

### See Also

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


