---
title: GradientFill.SetPresetThemeGradient
second_title: Aspose.Cells for .NET API Reference
description: GradientFill method. Sets preset theme gradient fill
type: docs
url: /net/aspose.cells.drawing/gradientfill/setpresetthemegradient/
---
## GradientFill.SetPresetThemeGradient method

Sets preset theme gradient fill.

```csharp
public void SetPresetThemeGradient(PresetThemeGradientType gradientType, 
    ThemeColorType themeColorType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| gradientType | PresetThemeGradientType | The preset gradient type. |
| themeColorType | ThemeColorType | The theme color type. |

### Examples

```csharp
// Called: shape.Fill.GradientFill.SetPresetThemeGradient(PresetThemeGradientType.BottomSpotlight, ThemeColorType.Accent5);
[Test]
        public void Method_ThemeColorType_()
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

* enum [PresetThemeGradientType](../../presetthemegradienttype/)
* enum [ThemeColorType](../../../aspose.cells/themecolortype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


