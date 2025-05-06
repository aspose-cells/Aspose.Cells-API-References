---
title: DeleteBlankOptions.EndIndex
second_title: Aspose.Cells for .NET API Reference
description: DeleteBlankOptions property. Specifies the end row/column indexinclusive of the range to check and delete blank rows/columns. Default value is 1 and 1 means the maximum range of all objectscells drawings ... that need to be checked
type: docs
url: /net/aspose.cells/deleteblankoptions/endindex/
---
## DeleteBlankOptions.EndIndex property

Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked.

```csharp
public int EndIndex { get; set; }
```

### Examples

```csharp
// Called: dbo.EndIndex = 7;
[Test]
        public void Property_EndIndex()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[1, 0];
            cells.DeleteBlankColumns();
            foreach (Cell c in cells)
            {
                Assert.Fail(c.Name + &quot; is not null, corresponding row should be deleted.&quot;);
            }
            cells[0, 2].PutValue(2);
            cells[0, 5].PutValue(5);
            cells[0, 9].PutValue(9);
            DeleteBlankOptions dbo = new DeleteBlankOptions();
            dbo.StartIndex = 4;
            dbo.EndIndex = 7;
            cells.DeleteBlankColumns(dbo);
            FormulaCaseUtil.AssertInt(2, cells[0, 2].Value, &quot;C1&quot;);
            FormulaCaseUtil.AssertInt(5, cells[0, 4].Value, &quot;G1-&gt;F1&quot;);
            FormulaCaseUtil.AssertInt(9, cells[0, 6].Value, &quot;K1-&gt;G1&quot;);
        }
```

### See Also

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


