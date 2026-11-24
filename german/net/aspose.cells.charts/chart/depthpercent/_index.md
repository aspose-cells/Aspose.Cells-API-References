---
title: "Chart.DepthPercent"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart‑Eigenschaft. Gibt die Tiefe eines 3D‑Diagramms als Prozentsatz der Diagrammbreite zwischen 20 % und 2000 % an."
type: docs
url: /de/net/aspose.cells.charts/chart/depthpercent/
---
## Chart.DepthPercent property

Stellt die Tiefe eines 3‑D‑Diagramms als Prozentsatz der Diagrammbreite dar (zwischen 20 % und 2000 %).

```csharp
public int DepthPercent { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyDepthPercentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // Ein 3D‑Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Setzen Sie die DepthPercent‑Eigenschaft (steuert die Tiefe eines 3D‑Diagramms als Prozentsatz der Diagrammbreite)
            chart.DepthPercent = 150; // 150% depth

            // Speichere die Arbeitsmappe
            workbook.Save("ChartDepthPercentDemo.xlsx");

            Console.WriteLine("Chart with DepthPercent 150% created successfully.");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


