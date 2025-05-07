---
title: DeleteBlankOptions.StartIndex
second_title: Aspose.Cells for .NET API Reference
description: DeleteBlankOptions property. Specifies the start row/column index of the range to check and delete blank rows/columns
type: docs
url: /net/aspose.cells/deleteblankoptions/startindex/
---
## DeleteBlankOptions.StartIndex property

Specifies the start row/column index of the range to check and delete blank rows/columns.

```csharp
public int StartIndex { get; set; }
```

### Examples

```csharp
// Called: dbo.StartIndex = 4;
[Test]
        public void Property_StartIndex()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[1, 0];
            cells.DeleteBlankRows();
            foreach(Cell c in cells)
            {
                Assert.Fail(c.Name + " is not null, corresponding row should be deleted.");
            }
            cells[2, 0].PutValue(2);
            cells[5, 0].PutValue(5);
            cells[9, 0].PutValue(9);
            DeleteBlankOptions dbo = new DeleteBlankOptions();
            dbo.StartIndex = 4;
            dbo.EndIndex = 7;
            cells.DeleteBlankRows(dbo);
            FormulaCaseUtil.AssertInt(2, cells[2, 0].Value, "A3");
            FormulaCaseUtil.AssertInt(5, cells[4, 0].Value, "A6->A5");
            FormulaCaseUtil.AssertInt(9, cells[6, 0].Value, "A10->A7");
        }
```

### See Also

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


