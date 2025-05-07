---
title: GradientStop.Position
second_title: Aspose.Cells for .NET API Reference
description: GradientStop property. The position of the stop
type: docs
url: /net/aspose.cells.drawing/gradientstop/position/
---
## GradientStop.Position property

The position of the stop.

```csharp
public double Position { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(46, shape.Fill.GradientFill.GradientStops[1].Position);
[Test]
        public void Property_Position()
        {
            Workbook workbook = new Workbook();
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            Shape shape = shapes[0];

            shape.Fill.FillType = FillType.Gradient;
            shape.Fill.GradientFill.SetPresetThemeGradient(PresetThemeGradientType.BottomSpotlight, ThemeColorType.Accent5);
            Assert.AreEqual(46, shape.Fill.GradientFill.GradientStops[1].Position);
            workbook.Save(Constants.destPath + "CellsNet51925.xlsx");
        }
```

### See Also

* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


