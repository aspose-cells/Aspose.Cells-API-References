---
title: ChartGlobalizationSettings.GetOtherName
second_title: Aspose.Cells for .NET API Reference
description: ChartGlobalizationSettings method. Gets the name of Other labels for Chart
type: docs
url: /net/aspose.cells.charts/chartglobalizationsettings/getothername/
---
## ChartGlobalizationSettings.GetOtherName method

Gets the name of "Other" labels for Chart.

```csharp
public virtual string GetOtherName()
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetOtherNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Add chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Create globalization settings and get other name
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string otherName = globalizationSettings.GetOtherName();

            // Output the result
            Console.WriteLine("Other Name: " + otherName);

            // Save workbook
            workbook.Save("ChartGlobalizationDemo.xlsx");
        }
    }
}
```

### See Also

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


