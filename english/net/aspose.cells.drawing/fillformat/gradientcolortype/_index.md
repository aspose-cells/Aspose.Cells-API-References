---
title: FillFormat.GradientColorType
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Returns the gradient color type for the specified fill
type: docs
url: /net/aspose.cells.drawing/fillformat/gradientcolortype/
---
## FillFormat.GradientColorType property

Returns the gradient color type for the specified fill.

```csharp
public GradientColorType GradientColorType { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(GradientColorType.TwoColors, point.Area.FillFormat.GradientColorType, "chart.NSeries[0].Area.FillFormat.GradientColorType");
private void FillFormat_Property_GradientColorType(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
           // Series aseries = chart.NSeries[1];
            ChartPoint point = chart.NSeries[0].Points[1];
            AssertHelper.AreEqual(GradientColorType.TwoColors, point.Area.FillFormat.GradientColorType, "chart.NSeries[0].Area.FillFormat.GradientColorType");
        }
```

### See Also

* enum [GradientColorType](../../gradientcolortype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


