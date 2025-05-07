---
title: Axis.IsDisplayUnitLabelShown
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents if the display unit label is shown on the specified axis
type: docs
url: /net/aspose.cells.charts/axis/isdisplayunitlabelshown/
---
## Axis.IsDisplayUnitLabelShown property

Represents if the display unit label is shown on the specified axis.

```csharp
public bool IsDisplayUnitLabelShown { get; set; }
```

### Remarks

The default value is True.

### Examples

```csharp
// Called: chart.ValueAxis.IsDisplayUnitLabelShown = true;
public static void Property_IsDisplayUnitLabelShown()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Add a new worksheet to the workbook
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Add some sample data to the worksheet
            worksheet.Cells["A1"].PutValue(500000);
            worksheet.Cells["A2"].PutValue(1000000);
            worksheet.Cells["A3"].PutValue(1500000);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Add NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Set the display unit of the value axis to Millions
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            
            // Optionally, show the display unit label
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Save the workbook
            workbook.Save("DisplayUnitTypeExample.xlsx");
            workbook.Save("DisplayUnitTypeExample.pdf");
        }
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


