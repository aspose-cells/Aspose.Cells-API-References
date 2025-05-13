---
title: ShapeCollection.UpdateSelectedValue
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Update the selected value by the value of the linked cell or range of the shape
type: docs
url: /net/aspose.cells.drawing/shapecollection/updateselectedvalue/
---
## ShapeCollection.UpdateSelectedValue method

Update the selected value by the value of the linked cell or range of the shape.

```csharp
public void UpdateSelectedValue()
```

### Examples

```csharp
// Called: w.Worksheets[1].Shapes.UpdateSelectedValue();
public void ShapeCollection_Method_UpdateSelectedValue()
{
    Workbook w = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual(1,w.Worksheets.ActiveSheetIndex);
    w.Worksheets[1].Shapes.UpdateSelectedValue();
    Assert.AreEqual(1, w.Worksheets.ActiveSheetIndex);
}
```

### See Also

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


