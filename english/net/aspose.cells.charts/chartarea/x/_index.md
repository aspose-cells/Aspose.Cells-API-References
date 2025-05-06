---
title: ChartArea.X
second_title: Aspose.Cells for .NET API Reference
description: ChartArea property. Gets or gets the horizontal offset from its upper left corner column in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/chartarea/x/
---
## ChartArea.X property

Gets or gets the horizontal offset from its upper left corner column, in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use ChartArea.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Please use ChartArea.XRatioToChart property, instead. X = XRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: chartArea.X = 10;
public static void Property_X()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Adding a sample value to &quot;A1&quot; cell
            worksheet.Cells[&quot;A1&quot;].PutValue(50);

            // Adding a sample value to &quot;A2&quot; cell
            worksheet.Cells[&quot;A2&quot;].PutValue(100);

            // Adding a sample value to &quot;A3&quot; cell
            worksheet.Cells[&quot;A3&quot;].PutValue(150);

            // Adding a sample value to &quot;B1&quot; cell
            worksheet.Cells[&quot;B1&quot;].PutValue(60);

            // Adding a sample value to &quot;B2&quot; cell
            worksheet.Cells[&quot;B2&quot;].PutValue(32);

            // Adding a sample value to &quot;B3&quot; cell
            worksheet.Cells[&quot;B3&quot;].PutValue(50);

            // Adding a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);

            // Accessing the instance of the newly added chart
            Chart chart = worksheet.Charts[chartIndex];

            // Adding NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B3&quot;
            chart.NSeries.Add(&quot;A1:B3&quot;, true);

            // Getting Chart Area
            ChartArea chartArea = chart.ChartArea;

            // Setting properties of ChartArea
            chartArea.X = 10;
            chartArea.Y = 10;
            chartArea.Width = 400;
            chartArea.Height = 300;
            chartArea.IsInnerMode = false;
            chartArea.AutoScaleFont = true;
            chartArea.BackgroundMode = BackgroundMode.Transparent;
            chartArea.IsAutomaticSize = true;
            chartArea.Shadow = true;

            // Setting the foreground color of the chart area
            chartArea.Area.ForegroundColor = Color.Yellow;

            // Saving the Excel file
            workbook.Save(&quot;ChartAreaExample.xlsx&quot;);
            workbook.Save(&quot;ChartAreaExample.pdf&quot;);
        }
```

### See Also

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


