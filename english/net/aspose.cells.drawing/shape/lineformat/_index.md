---
title: Shape.LineFormat
second_title: Aspose.Cells for .NET API Reference
description: Shape property. Returns a MsoLineFormat object that contains line formatting properties for the specified shape
type: docs
url: /net/aspose.cells.drawing/shape/lineformat/
---
## Shape.LineFormat property

Returns a MsoLineFormat object that contains line formatting properties for the specified shape.

```csharp
[Obsolete("Use Shape.Line property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoLineFormat LineFormat { get; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use Shape.Line property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: rectangle.LineFormat.Weight = 3;
public void Shape_Property_LineFormat()
{
    Workbook excelbook = new Workbook();
    //Add a rectangle control.
    Aspose.Cells.Drawing.RectangleShape rectangle = excelbook.Worksheets[0].Shapes.AddRectangle(3, 0, 2, 0, 70, 130);
    //Set the placement of the rectangle.
    rectangle.Placement = PlacementType.FreeFloating;
    rectangle.Fill.FillType = FillType.Solid;
    //Set the fill format.
    rectangle.Fill.SolidFill.Color = System.Drawing.Color.FromArgb(0, 0, 255);
    //Set the line weight.
    rectangle.LineFormat.Weight = 3;
    //Set the fill transparency
    //  rectangle.Fill.Transparency = 0;
    //Set the color of the line.
    rectangle.Line.SolidFill.Color = System.Drawing.Color.FromArgb(0, 0, 255);//The border color would be a bit darker instead of normal blue

    //Set the dash style of the rectangle.
    rectangle.Line.DashStyle = MsoLineDashStyle.Solid;

    excelbook.Save(Constants.destPath + "example.xlsx");
    Workbook workbook = new Workbook(Constants.destPath + "example.xlsx");
    Shape shape = workbook.Worksheets[0].Shapes[0];
   AssertHelper.AreEqual(shape.Line.SolidFill.Color, System.Drawing.Color.FromArgb(0, 0, 255));

}
```

### See Also

* class [MsoLineFormat](../../msolineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


