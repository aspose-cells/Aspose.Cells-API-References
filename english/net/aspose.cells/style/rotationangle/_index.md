---
title: Style.RotationAngle
second_title: Aspose.Cells for .NET API Reference
description: Style property. Represents text rotation angle
type: docs
url: /net/aspose.cells/style/rotationangle/
---
## Style.RotationAngle property

Represents text rotation angle.

```csharp
public int RotationAngle { get; set; }
```

### Remarks

0: Not rotated.

255: Top to Bottom.

-90: Downward.

90: Upward.

You can set 255 or value ranged from -90 to 90.

### Examples

```csharp
// Called: Assert.AreEqual(255, style.RotationAngle);
public void Style_Property_RotationAngle()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Style style = workbook.Worksheets[0].Cells["B2"].GetStyle();
    Assert.AreEqual(-90, style.RotationAngle);
    style = workbook.Worksheets[0].Cells["C3"].GetStyle();
    Assert.AreEqual(90, style.RotationAngle);
    style = workbook.Worksheets[0].Cells["D4"].GetStyle();
    Assert.AreEqual(255, style.RotationAngle);
    style = workbook.Worksheets[0].Cells["E6"].GetStyle();
    Assert.AreEqual(0, style.RotationAngle);
    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


