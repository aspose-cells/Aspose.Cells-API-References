---
title: Axis.CategoryType
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the type of the category axis
type: docs
url: /net/aspose.cells.charts/axis/categorytype/
---
## Axis.CategoryType property

Represents the type of the category axis.

```csharp
public CategoryType CategoryType { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCategoryTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add sample data
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                sheet.Cells["B" + i].PutValue(i * 10);
            }

            // Add a chart
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 2, 25, 11);
            Chart chart = sheet.Charts[chartIndex];
            
            // Set chart data source
            chart.NSeries.Add("=Sheet1!$A$1:$B$10", true);

            // Demonstrate CategoryType property
            chart.CategoryAxis.CategoryType = Aspose.Cells.Charts.CategoryType.AutomaticScale;
            Console.WriteLine("CategoryType set to AutomaticScale");

            // Save the workbook
            workbook.Save("AxisPropertyCategoryTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### See Also

* enum [CategoryType](../../categorytype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


