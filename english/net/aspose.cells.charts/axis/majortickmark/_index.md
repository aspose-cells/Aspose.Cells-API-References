---
title: Axis.MajorTickMark
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the type of major tick mark for the specified axis
type: docs
url: /net/aspose.cells.charts/axis/majortickmark/
---
## Axis.MajorTickMark property

Represents the type of major tick mark for the specified axis.

```csharp
public TickMarkType MajorTickMark { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorTickMarkDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add sample data for the chart
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Add a column chart
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Set chart data source
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Set major tick mark type to outside
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            // Save the workbook
            workbook.Save("AxisPropertyMajorTickMarkDemo_out.xlsx");
        }
    }
}
```

### See Also

* enum [TickMarkType](../../tickmarktype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


