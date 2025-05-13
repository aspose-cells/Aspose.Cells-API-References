---
title: Class SolidFill
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.SolidFill class. Encapsulates the object that represents solid fill format
type: docs
url: /net/aspose.cells.drawing/solidfill/
---
## SolidFill class

Encapsulates the object that represents solid fill format

```csharp
public class SolidFill : Fill
```

## Properties

| Name | Description |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/solidfill/cellscolor/) { get; set; } | Gets and sets the [`CellsColor`](./cellscolor/) object. |
| [Color](../../aspose.cells.drawing/solidfill/color/) { get; set; } | Gets or sets the Color. |
| [Transparency](../../aspose.cells.drawing/solidfill/transparency/) { get; set; } | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/solidfill/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/solidfill/gethashcode/)() | Gets the hash code. |

### Examples

```csharp
// Called: SolidFill fill = font.Fill.SolidFill;
public void Drawing_Type_SolidFill()
{

    Workbook workbook = new Workbook();
    Worksheet sheet = workbook.Worksheets[0];
    Shape sp = sheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 4, 4, 4, 4, 100, 700);
    sp.Fill.FillType = FillType.None;

    sp.Text = "Hello World !!!";
    FontSetting fs = sp.Characters(0, "Hello World !!!".Length);
    TextOptions font = fs.TextOptions;
    font.Name = "Calibri";
    font.Size = 54;
    font.IsBold = true;


    font.Color = System.Drawing.Color.Green;
    font.Outline.FillType = FillType.Solid;
    SolidFill outLineFill = (SolidFill)font.Outline.SolidFill;
    outLineFill.Color = Color.White;

    font.Fill.FillType = FillType.Solid;
    SolidFill fill = font.Fill.SolidFill;
    fill.Color = Color.Green;
    font.Shadow.PresetType = PresetShadowType.OffsetBottom;

    Util.SaveManCheck(workbook, "Shape", "example.xlsx");
}
```

### See Also

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


