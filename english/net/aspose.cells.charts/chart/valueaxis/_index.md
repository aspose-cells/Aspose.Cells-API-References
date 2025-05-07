---
title: Chart.ValueAxis
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the charts Y axis
type: docs
url: /net/aspose.cells.charts/chart/valueaxis/
---
## Chart.ValueAxis property

Gets the chart's Y axis.

```csharp
public Axis ValueAxis { get; }
```

### Examples

```csharp
// Called: chart.ValueAxis.MajorTickMark = TickMarkType.Outside;
[Test]
        public void Property_ValueAxis()
        {
            Workbook workbook = new Workbook();
            workbook = TestColumn.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            checkTickMarkType_Outside(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkTickMarkType_Outside(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkTickMarkType_Outside(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


