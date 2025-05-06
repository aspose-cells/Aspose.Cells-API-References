---
title: Chart.ChartArea
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the chart area in the worksheet
type: docs
url: /net/aspose.cells.charts/chart/chartarea/
---
## Chart.ChartArea property

Gets the chart area in the worksheet.

```csharp
public ChartArea ChartArea { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(FillType.Gradient, chart.ChartArea.Area.FillFormat.FillType, &amp;quot;chart.ChartArea.Area.FillFormat.FillType&amp;quot;);
private void Property_ChartArea(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(FillType.Gradient, chart.ChartArea.Area.FillFormat.FillType, &quot;chart.ChartArea.Area.FillFormat.FillType&quot;);
        }
```

### See Also

* class [ChartArea](../../chartarea/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


