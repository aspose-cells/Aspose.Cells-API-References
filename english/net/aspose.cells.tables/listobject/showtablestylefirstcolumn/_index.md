---
title: ListObject.ShowTableStyleFirstColumn
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Indicates whether the first column in the table should have the style applied
type: docs
url: /net/aspose.cells.tables/listobject/showtablestylefirstcolumn/
---
## ListObject.ShowTableStyleFirstColumn property

Indicates whether the first column in the table should have the style applied.

```csharp
public bool ShowTableStyleFirstColumn { get; set; }
```

### Examples

```csharp
// Called: listObjects[0].ShowTableStyleFirstColumn = true;
public void ListObject_Property_ShowTableStyleFirstColumn()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells[0, 0].PutValue("a");
    cells[1, 0].PutValue(1);
    cells[2, 0].PutValue(2);
    cells[3, 0].PutValue(3);
    cells[0, 1].PutValue("b");
    cells[1, 1].PutValue(4);
    cells[2, 1].PutValue(5);
    cells[3, 1].PutValue(6);

    ListObjectCollection listObjects = workbook.Worksheets[0].ListObjects;
    listObjects.Add("A1", "B4", true);
    listObjects[0].ShowTableStyleFirstColumn = true;
    workbook.Save(Constants.destPath + "testListObject.xlsx", SaveFormat.Xlsx);

    workbook = new Workbook(Constants.destPath + "testListObject.xlsx");
    listObjects = workbook.Worksheets[0].ListObjects;
    ListObject listObject = listObjects[0];
    AssertHelper.AreEqual(true, listObject.ShowTableStyleFirstColumn, "listObject.ShowTableStyleFirstColumn");
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


