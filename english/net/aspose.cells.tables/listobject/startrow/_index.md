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
// Called: Assert.AreEqual( wbktmp.Worksheets[0].ListObjects[0].StartRow,2);
public void ListObject_Property_StartRow()
{
    var wbk = new Workbook(Constants.sourcePath + "example.xlsx");
    var wbktmp = new Workbook();
    wbktmp.Worksheets[0].Cells.CreateRange(0, 0, 9, 4).Copy(wbk.Worksheets[0].Cells.CreateRange(2, 0, 9, 4));

  Assert.AreEqual( wbktmp.Worksheets[0].ListObjects[0].StartRow,2);

    wbktmp = new Workbook();
    wbktmp.Worksheets[0].Cells.CreateRange(0, 0, 100, 100).Copy(wbk.Worksheets[0].Cells.CreateRange(0, 0, 100, 100));

    Assert.AreEqual(wbktmp.Worksheets[0].ListObjects[0].StartRow, 4);
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


