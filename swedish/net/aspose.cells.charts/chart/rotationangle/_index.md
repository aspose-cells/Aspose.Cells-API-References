---
title: "Chart.RotationAngle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart egenskap. Representerar rotationen av 3D-diagramvyn, rotationen av plotområdet kring z-axeln i grader"
type: docs
url: /sv/net/aspose.cells.charts/chart/rotationangle/
---
## Chart.RotationAngle property

Representerar rotationen av 3‑D-diagramvyn (rotationen av plotområdet runt z‑axeln, i grader).

```csharp
public int RotationAngle { get; set; }
```

### Anmärkningar

Värdet för denna egenskap måste vara från 0 till 360, förutom för 3D-stapeldiagram, där värdet måste vara från 0 till 44. Standardvärdet är 20. Gäller endast för 3D-diagram.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyRotationAngleDemo
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
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett 3D-kolumndiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ange rotationsvinkeln till 45 grader
            chart.RotationAngle = 45;

            // Spara arbetsboken
            workbook.Save("ChartRotationAngleDemo.xlsx");

            Console.WriteLine("Chart with rotation angle created successfully.");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


