---
title: Enum FillType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.FillType enum. Fill format type
type: docs
url: /net/aspose.cells.drawing/filltype/
---
## FillType enumeration

Fill format type.

```csharp
public enum FillType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Automatic | `0` | Represents automatic formatting type. |
| None | `1` | Represents none formatting type. |
| Solid | `2` | Solid fill format. |
| Gradient | `3` | Gradient fill format. |
| Texture | `4` | Texture fill format(includes picture fill). |
| Pattern | `5` | Pattern fill format. |
| Group | `6` | Inherit the fill properties of the group. |

### Examples

```csharp
// Called: Assert.AreEqual(shape.Fill.FillType, FillType.Gradient);
public void Drawing_Type_FillType()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm");
    Shape shape = workbook.Worksheets["1.1 Antenna System (RF)"].Shapes["Rectangle 1184"];
    Assert.AreEqual(shape.Fill.FillType, FillType.Gradient);
    workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    shape = workbook.Worksheets[0].Shapes["TextBox 1"];
    Assert.AreEqual(shape.Fill.FillType, FillType.Gradient);
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


