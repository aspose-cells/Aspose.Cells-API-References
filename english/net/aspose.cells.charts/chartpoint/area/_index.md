---
title: ChartPoint.Area
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. Gets the  area
type: docs
url: /net/aspose.cells.charts/chartpoint/area/
---
## ChartPoint.Area property

Gets the ` area`.

```csharp
public Area Area { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(GradientColorType.TwoColors, point.Area.FillFormat.GradientColorType, &amp;quot;chart.NSeries[0].Area.FillFormat.GradientColorType&amp;quot;);
private void Property_Area(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
           // Series aseries = chart.NSeries[1];
            ChartPoint point = chart.NSeries[0].Points[1];
            AssertHelper.AreEqual(GradientColorType.TwoColors, point.Area.FillFormat.GradientColorType, &quot;chart.NSeries[0].Area.FillFormat.GradientColorType&quot;);
        }
```

### See Also

* class [Area](../../../aspose.cells.drawing/area/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


