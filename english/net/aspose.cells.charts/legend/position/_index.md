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
// Called: chart.Legend.Position = LegendPositionType.Left;
[Test]
        public void Property_Position()
        {
            Workbook workbook = new Workbook();
            workbook = TestColumn.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.Legend.Position = LegendPositionType.Left;

            checkLegendPositionType_Left(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkLegendPositionType_Left(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkLegendPositionType_Left(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [LegendPositionType](../../legendpositiontype/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


