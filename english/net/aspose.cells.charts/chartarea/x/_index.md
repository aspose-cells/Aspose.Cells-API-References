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
public static void ChartArea_Property_X()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Adding a sample value to "A1" cell
            worksheet.Cells["A1"].PutValue(50);

            // Adding a sample value to "A2" cell
            worksheet.Cells["A2"].PutValue(100);

            // Adding a sample value to "A3" cell
            worksheet.Cells["A3"].PutValue(150);

            // Adding a sample value to "B1" cell
            worksheet.Cells["B1"].PutValue(60);

            // Adding a sample value to "B2" cell
            worksheet.Cells["B2"].PutValue(32);

            // Adding a sample value to "B3" cell
            worksheet.Cells["B3"].PutValue(50);

            // Adding a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);

            // Accessing the instance of the newly added chart
            Chart chart = worksheet.Charts[chartIndex];

            // Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
            chart.NSeries.Add("A1:B3", true);

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
            workbook.Save("ChartAreaExample.xlsx");
            workbook.Save("ChartAreaExample.pdf");
        }
```

### See Also

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


