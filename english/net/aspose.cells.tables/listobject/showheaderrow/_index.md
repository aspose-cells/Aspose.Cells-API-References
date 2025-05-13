---
title: ListObject.ShowHeaderRow
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets whether this ListObject show header row
type: docs
url: /net/aspose.cells.tables/listobject/showheaderrow/
---
## ListObject.ShowHeaderRow property

Gets and sets whether this ListObject show header row.

```csharp
public bool ShowHeaderRow { get; set; }
```

### Examples

```csharp
// Called: tbl.ShowHeaderRow = false;
public void ListObject_Property_ShowHeaderRow()
{
    Workbook wb = new Workbook();
    wb.Worksheets.Add();
    Worksheet ws = wb.Worksheets[0];

    ws.Cells[0, 0].PutValue("TITLE"); // Not in table
    ws.Cells[1, 0].PutValue("COLHEADER"); // header Row
    ws.Cells[2, 0].PutValue("ROW1");
    ws.Cells[3, 0].PutValue("ROW1");

    int index = ws.ListObjects.Add(1, 0, 3, 0, true);
    Aspose.Cells.Tables.ListObject tbl = ws.ListObjects[index];
    tbl.DisplayName = "TABLE";
    tbl.TableStyleType = Aspose.Cells.Tables.TableStyleType.None;
    tbl.UpdateColumnName();
           
    tbl.ShowHeaderRow = false;
    Assert.AreEqual(ws.Cells[1, 0].StringValue, "");

}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


