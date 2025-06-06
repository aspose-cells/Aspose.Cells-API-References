---
title: AxisBins.ResetUnderflow
second_title: Aspose.Cells for .NET API Reference
description: AxisBins method. Reset the underflow
type: docs
url: /net/aspose.cells.charts/axisbins/resetunderflow/
---
## AxisBins.ResetUnderflow method

Reset the underflow

```csharp
[Obsolete("This is an internal method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ResetUnderflow()
```

### Remarks

NOTE: This method is now obsolete. This is an internal method that does not need to be called externally to avoid causing problems. This property will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisBinsMethodResetUnderflowDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Create a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Get the value axis
            Axis valueAxis = chart.ValueAxis;
            
            // Create axis bins
            valueAxis.Bins.IsAutomatic = false;
            valueAxis.Bins.Count = 5;
            valueAxis.Bins.Underflow = 5;
            
            try
            {
                // Call the ResetUnderflow method
                valueAxis.Bins.ResetUnderflow();
                
                Console.WriteLine("Underflow value after reset: " + valueAxis.Bins.Underflow);
                
                // Save the workbook
                workbook.Save("AxisBinsMethodResetUnderflowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetUnderflow method: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


