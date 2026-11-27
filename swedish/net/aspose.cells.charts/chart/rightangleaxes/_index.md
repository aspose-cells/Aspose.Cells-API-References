---
title: "Chart.RightAngleAxes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagramegenskap. Sant om diagrammets axlar är i räta vinklar. Gäller endast för 3D-diagram förutom Column3D och 3D-pi-diagram"
type: docs
url: /sv/net/aspose.cells.charts/chart/rightangleaxes/
---
## Chart.RightAngleAxes property

True om diagramaxlarna är vinkelräta. Gäller endast för 3‑D-diagram (förutom Column3D och 3‑D-pie-diagram).

```csharp
public bool RightAngleAxes { get; set; }
```

### Anmärkningar

Om denna egenskap är sann, ignoreras Perspective-egenskapen.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyRightAngleAxesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Lägg till ett 3D-kolumndiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demonstrera RightAngleAxes-egenskapen
            chart.RightAngleAxes = true;
            Console.WriteLine("RightAngleAxes is set to: " + chart.RightAngleAxes);

            // Spara arbetsboken
            workbook.Save("RightAngleAxesDemo.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


