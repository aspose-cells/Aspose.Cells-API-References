---
title: "Chart.Elevation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Diagramm-Eigenschaft. Stellt die Elevation der 3D-Diagrammansicht in Grad dar"
type: docs
url: /de/net/aspose.cells.charts/chart/elevation/
---
## Chart.Elevation property

Stellt die Elevation der 3‑D‑Diagrammansicht in Grad dar.

```csharp
public int Elevation { get; set; }
```

### Hinweise

Die Diagrammhöhe ist die Höhe, aus der Sie das Diagramm betrachten, in Grad. Der Standardwert ist 15 für die meisten Diagrammtypen. Der Wert dieser Eigenschaft muss zwischen -90 und 90 liegen, außer bei 3‑D‑Balkendiagrammen, wo er zwischen 0 und 44 liegen muss.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Ein 3D‑Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Setzen Sie die Elevation‑Eigenschaft (Winkel in Grad)
            chart.Elevation = 30;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartElevationDemo.xlsx");

            Console.WriteLine("Chart created with elevation set to 30 degrees.");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


