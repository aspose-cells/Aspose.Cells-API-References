---
title: Legend.Position
second_title: Aspose.Cells for .NET API Reference
description: Legend property. Gets or sets the legend position type
type: docs
url: /net/aspose.cells.charts/legend/position/
---
## Legend.Position property

Gets or sets the legend position type.

```csharp
public LegendPositionType Position { get; set; }
```

### Remarks

Default position is right.If the legend is at left or right side of the chart, setting Legend.X property will not take effect.If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.

### Examples

```csharp
// Called: AssertHelper.AreEqual(LegendPositionType.Left, chart.Legend.Position, "chart.Legend.Position");
private void Legend_Property_Position(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(LegendPositionType.Left, chart.Legend.Position, "chart.Legend.Position");
        }
```

### See Also

* enum [LegendPositionType](../../legendpositiontype/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


