---
title: "ChartPoint.YValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Liest oder setzt den Y-Wert des Diagrammpunkts"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/yvalue/
---
## ChartPoint.YValue property

Liest oder setzt den Y‑Wert des Diagrammpunkts.

```csharp
public object YValue { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyYValueDemo
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
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Erhalte die Punkte der ersten Serie
            Series series = chart.NSeries[0];
            var points = series.Points;

            // Demonstriere die YValue-Eigenschaft
            Console.WriteLine("Y Values of Chart Points:");
            for (int i = 0; i < points.Count; i++)
            {
                Console.WriteLine($"Point {i + 1}: {points[i].YValue}");
            }

            // Ändere den YValue eines Punktes
            points[2].YValue = 50;
            Console.WriteLine($"\nModified Point 3 YValue to: {points[2].YValue}");

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointYValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


