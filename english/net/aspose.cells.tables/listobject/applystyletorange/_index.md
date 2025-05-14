---
title: ListObject.ApplyStyleToRange
second_title: Aspose.Cells for .NET API Reference
description: ListObject method. Apply the table style to the range
type: docs
url: /net/aspose.cells.tables/listobject/applystyletorange/
---
## ListObject.ApplyStyleToRange method

Apply the table style to the range.

```csharp
public void ApplyStyleToRange()
```

### Examples

```csharp
// Called: listObject.ApplyStyleToRange();
public void ListObject_Method_ApplyStyleToRange()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    ListObject listObject = workbook.Worksheets[0].ListObjects[0];
    listObject.ApplyStyleToRange();
    Style style = workbook.Worksheets[0].Cells["A1"].GetStyle();
    Assert.AreEqual(style.ForegroundColor.ToArgb() & 0xFFFFFF, System.Drawing.Color.FromArgb(79, 129, 189).ToArgb() & 0xFFFFFF);
                
    workbook.Worksheets[0].ListObjects.RemoveAt(0);
    workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    listObject = workbook.Worksheets[0].ListObjects[0];
    listObject.ConvertToRange();
    style = workbook.Worksheets[0].Cells["A1"].GetStyle();
    Assert.AreEqual(style.ForegroundColor.ToArgb() & 0xFFFFFF, System.Drawing.Color.FromArgb(79, 129, 189).ToArgb() & 0xFFFFFF);
    Assert.AreEqual(workbook.Worksheets[0].ListObjects.Count, 0);
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


