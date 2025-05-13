---
title: ListObject.ShowTotals
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets whether this ListObject show total row
type: docs
url: /net/aspose.cells.tables/listobject/showtotals/
---
## ListObject.ShowTotals property

Gets and sets whether this ListObject show total row.

```csharp
public bool ShowTotals { get; set; }
```

### Examples

```csharp
// Called: table.ShowTotals = true;
public void ListObject_Property_ShowTotals()
{
    var loadPath = Path.Combine(Constants.sourcePath, "example.xlsx");
    var mybook = new Workbook(loadPath);
    var table = mybook.Worksheets[0].ListObjects[0];
    table.ShowTotals = false;
    table.ShowTotals = true;
    Assert.AreEqual("Ergebnis", mybook.Worksheets[0].Cells["C8"].StringValue);
    Assert.IsTrue(mybook.Worksheets[0].Cells["E8"].IsFormula);
    Util.SaveForViewer(mybook, "13", "example.xlsx");
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


