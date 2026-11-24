---
title: "Walls.CenterY"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Walls-Eigenschaft. Gibt die y‑Koordinate der linken unteren Ecke des Wandzentrums in Einheiten von 1/4000 der Diagrammhöhe zurück, nachdem die Methode Chart.Calculate aufgerufen wurde."
type: docs
url: /de/net/aspose.cells.charts/walls/centery/
---
## Walls.CenterY property

Liest die y‑Koordinate der linken unteren Ecke des Wandzentrums in Einheiten von 1/4000 der Diagrammhöhe nach Aufruf der Methode Chart.Calculate().

```csharp
public int CenterY { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyCenterYDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein 3D‑Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column3D, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Berechnen Sie das Diagramm, um Eigenschaften zu aktualisieren
            chart.Calculate();

            // Greifen Sie auf walls zu und demonstrieren Sie die CenterY‑Eigenschaft
            Aspose.Cells.Charts.Walls walls = chart.Walls;
            Console.WriteLine("Wall CenterY position: " + walls.CenterY);

            // Speichere die Arbeitsmappe
            workbook.Save("WallsCenterYDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


