---
title: MsoLineFormat.Weight
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormat property. Returns or sets the weight of the line in units of pt
type: docs
url: /net/aspose.cells.drawing/msolineformat/weight/
---
## MsoLineFormat.Weight property

Returns or sets the weight of the line ,in units of pt.

```csharp
public double Weight { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Comments[0].CommentShape.LineFormat.Weight, 0.75);
public void MsoLineFormat_Property_Weight()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual(workbook.Worksheets[0].Comments[0].CommentShape.LineFormat.Weight, 0.75);
}
```

### See Also

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


