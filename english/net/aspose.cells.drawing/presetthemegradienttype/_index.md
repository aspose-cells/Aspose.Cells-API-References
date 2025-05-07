---
title: Enum PresetThemeGradientType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.PresetThemeGradientType enum. Represents the preset theme gradient type
type: docs
url: /net/aspose.cells.drawing/presetthemegradienttype/
---
## PresetThemeGradientType enumeration

Represents the preset theme gradient type.

```csharp
public enum PresetThemeGradientType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| LightGradient | `0` | Light gradient |
| TopSpotlight | `1` | Top spotlight |
| MediumGradient | `2` | Medium gradient |
| BottomSpotlight | `3` | Bottom spotlight |
| RadialGradient | `4` | Radial gradient |

### Examples

```csharp
// Called: shape.Fill.GradientFill.SetPresetThemeGradient(PresetThemeGradientType.BottomSpotlight, ThemeColorType.Accent5);
[Test]
        public void Type_PresetThemeGradientType()
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

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


