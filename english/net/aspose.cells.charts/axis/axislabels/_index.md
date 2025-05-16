---
title: Axis.AxisLabels
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Gets the labels of the axis after call Chart.Calculate method
type: docs
url: /net/aspose.cells.charts/axis/axislabels/
---
## Axis.AxisLabels property

Gets the labels of the axis after call Chart.Calculate() method.

```csharp
[Obsolete("Use Axis.GetAxisTexts method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList AxisLabels { get; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use Axis.GetAxisTexts method. This property will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples.AxisPropertyAxisLabelsDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyAxisLabelsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // Add a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Set chart data range
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Get the category axis
            Axis categoryAxis = chart.CategoryAxis;

            // Display current axis labels (using GetAxisTexts() instead of obsolete AxisLabels)
            Console.WriteLine("Current Axis Labels:");
            string[] axisLabels = categoryAxis.GetAxisTexts();
            foreach (string label in axisLabels)
            {
                Console.WriteLine(label);
            }

            // Change category axis properties that affect labels
            categoryAxis.CategoryType = CategoryType.AutomaticScale;
            categoryAxis.TickLabelPosition = TickLabelPositionType.Low;
            categoryAxis.TickLabelSpacing = 2;

            // Save the workbook
            workbook.Save("AxisLabelsDemo.xlsx");
        }
    }
}
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


