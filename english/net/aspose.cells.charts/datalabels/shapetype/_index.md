---
title: DataLabels.ShapeType
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets or sets shape type of data label
type: docs
url: /net/aspose.cells.charts/datalabels/shapetype/
---
## DataLabels.ShapeType property

Gets or sets shape type of data label.

```csharp
public DataLabelShapeType ShapeType { get; set; }
```

### Examples

```csharp
// Called: series.DataLabels.ShapeType = DataLabelShapeType.RoundRect;
public static void Property_ShapeType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;A&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;B&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;C&quot;);

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(10);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;B4&quot;].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the chart data range
            chart.SetChartDataRange(&quot;A1:B4&quot;, true);

            // Access the first series in the chart
            Series series = chart.NSeries[0];

            // Enable data labels for the series
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShapeType = DataLabelShapeType.RoundRect;

            // Save the workbook
            workbook.Save(&quot;DataLabelShapeTypeExample.xlsx&quot;);
            workbook.Save(&quot;DataLabelShapeTypeExample.pdf&quot;);
        }
```

### See Also

* enum [DataLabelShapeType](../../../aspose.cells.drawing/datalabelshapetype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


