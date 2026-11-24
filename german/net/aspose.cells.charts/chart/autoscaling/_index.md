---
title: "Chart.AutoScaling"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Wahr, wenn Microsoft Excel ein 3D-Diagramm so skaliert, dass es der Größe des entsprechenden 2D-Diagramms näher kommt. Die RightAngleAxes-Eigenschaft muss wahr sein"
type: docs
url: /de/net/aspose.cells.charts/chart/autoscaling/
---
## Chart.AutoScaling property

True, wenn Microsoft Excel ein 3‑D‑Diagramm skaliert, sodass es in der Größe dem entsprechenden 2‑D‑Diagramm näher kommt. Die Eigenschaft RightAngleAxes muss True sein.

```csharp
public bool AutoScaling { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyAutoScalingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // AutoScaling-Eigenschaft demonstrieren
            chart.AutoScaling = false;
            Console.WriteLine("Chart AutoScaling is set to: " + chart.AutoScaling);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartAutoScalingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


