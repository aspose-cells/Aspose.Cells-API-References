---
title: ListObject.StartRow
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets the start row of the range
type: docs
url: /net/aspose.cells.tables/listobject/startrow/
---
## ListObject.StartRow property

Gets the start row of the range.

```csharp
public int StartRow { get; }
```

### Examples

```csharp
// Called: Cell firstCell = table.DataRange.Worksheet.Cells[table.StartRow, table.StartColumn];
[Test]
        public void Property_StartRow()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet52749.xlsx");
            Worksheet ws = workbook.Worksheets[0];
            ListObject table = ws.ListObjects[0];
            Cell firstCell = table.DataRange.Worksheet.Cells[table.StartRow, table.StartColumn];

            table.Resize(firstCell.Row,
                         firstCell.Column,
                         table.EndRow,
                         table.EndColumn + 1,
                         false);

            ws.Cells.DeleteColumn(5);

            table.Resize(firstCell.Row,
                         firstCell.Column,
                         table.EndRow,
                         table.EndColumn + 1,
                         false);
            workbook.Save(Constants.destPath + "CellsNet52749.xlsx");
            Assert.AreEqual("Column102", table.ListColumns[table.ListColumns.Count - 1].Name);

           
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


