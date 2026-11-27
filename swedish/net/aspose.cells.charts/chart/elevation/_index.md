---
title: "Chart.Elevation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart egenskap. Representerar elevationen av 3D-diagramvyn i grader"
type: docs
url: /sv/net/aspose.cells.charts/chart/elevation/
---
## Chart.Elevation property

Representerar höjden på 3‑D‑diagramvyn, i grader.

```csharp
public int Elevation { get; set; }
```

### Anmärkningar

Diagramhöjden är den höjd där du visar diagrammet, i grader. Standardvärdet är 15 för de flesta diagramtyper. Värdet för den här egenskapen måste vara mellan -90 och 90, förutom för 3‑D stapeldiagram, där det måste vara mellan 0 och 44.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyElevationDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Lägg till ett 3D-kolumndiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ställ in höjd‑egenskapen (vinkel i grader)
            chart.Elevation = 30;
            
            // Spara arbetsboken
            workbook.Save("ChartElevationDemo.xlsx");

            Console.WriteLine("Chart created with elevation set to 30 degrees.");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


