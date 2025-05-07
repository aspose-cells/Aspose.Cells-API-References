---
title: Enum GradientColorType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.GradientColorType enum. Represents the gradient color type for the specified fill
type: docs
url: /net/aspose.cells.drawing/gradientcolortype/
---
## GradientColorType enumeration

Represents the gradient color type for the specified fill.

```csharp
public enum GradientColorType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No gradient color |
| OneColor | `1` | One gradient color |
| PresetColors | `2` | Preset gradient colors |
| TwoColors | `3` | Two gradient colors |

### Examples

```csharp
// Called: AssertHelper.AreEqual(GradientColorType.PresetColors, point.Area.FillFormat.GradientColorType, "chart.NSeries[0].Area.FillFormat.GradientColorType");
private void Type_GradientColorType(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            //Series aseries = chart.NSeries[2];
            ChartPoint point = chart.NSeries[0].Points[2];
            AssertHelper.AreEqual(GradientColorType.PresetColors, point.Area.FillFormat.GradientColorType, "chart.NSeries[0].Area.FillFormat.GradientColorType");
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


