---
title: Axis.CustomUnit
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Specifies a custom value for the display unit
type: docs
url: /net/aspose.cells.charts/axis/customunit/
---
## Axis.CustomUnit property

Specifies a custom value for the display unit.

```csharp
[Obsolete("Use Axis.CustomDisplayUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustomUnit { get; set; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use Axis.CustomDisplayUnit property. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples.AxisPropertyCustomUnitDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustomUnitDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for the chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);
            worksheet.Cells["B5"].PutValue(4000000);

            // Add a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Set chart data source
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Get the value axis
            Axis valueAxis = chart.ValueAxis;
            
            // Display current display unit settings
            Console.WriteLine("Current DisplayUnit: " + valueAxis.DisplayUnit);
            Console.WriteLine("Current CustomDisplayUnit: " + valueAxis.CustomDisplayUnit);
            
            // Set custom display unit (millions)
            valueAxis.DisplayUnit = DisplayUnitType.Custom;
            valueAxis.CustomDisplayUnit = 1000000; // 1 million
            valueAxis.IsDisplayUnitLabelShown = true;
            
            // Display the effect
            Console.WriteLine("After setting CustomDisplayUnit to 1,000,000");
            Console.WriteLine("Axis will now show values in millions (e.g., 1, 2, 3 instead of 1,000,000, 2,000,000)");
            
            // Save the workbook
            workbook.Save("AxisPropertyCustomUnitDemo.xlsx");
        }
    }
}
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


