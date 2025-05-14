---
title: ListObject.EndRow
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets the end row of the range
type: docs
url: /net/aspose.cells.tables/listobject/endrow/
---
## ListObject.EndRow property

Gets the end row of the range.

```csharp
public int EndRow { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(4, table.EndRow);
public void ListObject_Property_EndRow()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Cells cells = wb.Worksheets[0].Cells;
    ListObject table = wb.Worksheets[0].ListObjects[0];
    table.PutCellValue(5, 0, "88");
    table.PutCellValue(5, 1, 88);
    table.PutCellFormula(5, 2, "=C3");
    Assert.AreEqual(4, table.EndRow);

    wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


