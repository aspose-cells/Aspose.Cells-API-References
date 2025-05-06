---
title: ListObject.Resize
second_title: Aspose.Cells for .NET API Reference
description: ListObject method. Resize the range of the list object
type: docs
url: /net/aspose.cells.tables/listobject/resize/
---
## ListObject.Resize method

Resize the range of the list object.

```csharp
public void Resize(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row index of the new range. |
| startColumn | Int32 | The start column index of the new range. |
| endRow | Int32 | The end row index of the new range. |
| endColumn | Int32 | The end column index of the new range. |
| hasHeaders | Boolean | Whether this table has headers. |

### Examples

```csharp
// Called: table.Resize(firstCell.Row,
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet52749.xlsx&quot;);
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
            workbook.Save(Constants.destPath + &quot;CellsNet52749.xlsx&quot;);
            Assert.AreEqual(&quot;Column102&quot;, table.ListColumns[table.ListColumns.Count - 1].Name);

           
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


