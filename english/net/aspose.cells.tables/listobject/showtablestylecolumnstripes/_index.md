---
title: ListObject.ShowTableStyleColumnStripes
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Indicates whether column stripe formatting is applied
type: docs
url: /net/aspose.cells.tables/listobject/showtablestylecolumnstripes/
---
## ListObject.ShowTableStyleColumnStripes property

Indicates whether column stripe formatting is applied.

```csharp
public bool ShowTableStyleColumnStripes { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(false, listObject.ShowTableStyleColumnStripes, "listObject.ShowTableStyleColumnStripes");
public void ListObject_Property_ShowTableStyleColumnStripes()
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
    listObjects[0].ShowTableStyleColumnStripes = false;
    workbook.Save(Constants.destPath + "testListObject.xlsx", SaveFormat.Xlsx);

    workbook = new Workbook(Constants.destPath + "testListObject.xlsx");
    listObjects = workbook.Worksheets[0].ListObjects;
    ListObject listObject = listObjects[0];
    AssertHelper.AreEqual(false, listObject.ShowTableStyleColumnStripes, "listObject.ShowTableStyleColumnStripes");
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


