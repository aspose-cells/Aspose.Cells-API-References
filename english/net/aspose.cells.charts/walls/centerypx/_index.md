---
title: Walls.CenterYPx
second_title: Aspose.Cells for .NET API Reference
description: Walls property. Gets the y coordinate of the leftbottom corner of Wall center in units of pixels after calls Chart.Calculate method
type: docs
url: /net/aspose.cells.charts/walls/centerypx/
---
## Walls.CenterYPx property

Gets the y coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method.

```csharp
public int CenterYPx { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyCenterYPxDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            chart.Calculate();

            Walls walls = chart.Walls;
            Console.WriteLine("CenterYPx: " + walls.CenterYPx);

            workbook.Save("WallsPropertyCenterYPxDemo.xlsx");
        }
    }
}
```

### See Also

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


