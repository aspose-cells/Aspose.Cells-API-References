---
title: "ChartPoint.ArcStartPointXPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die x‑Koordinate des Startpunkts für das Kuchensegment zurück, nachdem die Methode Chart.Calculate aufgerufen wurde. Gilt für Kreis‑ und Donut‑Diagramme."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/arcstartpointxpx/
---
## ChartPoint.ArcStartPointXPx property

Ermittelt die x‑Koordinate des Startpunkts des Kuchensegments nach Aufruf der Methode Chart.Calculate(). Gilt für Kreis‑ und Donut‑Diagramme.

```csharp
public float ArcStartPointXPx { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcStartPointXPxDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ein Kreisdiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm berechnen, um sicherzustellen, dass Eigenschaften gefüllt sind.
            chart.Calculate();

            // Den ersten Diagrammpunkt abrufen
            ChartPoint point = chart.NSeries[0].Points[0];

            // Zeige den Wert von ArcStartPointXPx an
            Console.WriteLine("ArcStartPointXPx for first point: " + point.ArcStartPointXPx);

            // Hinweis: ArcStartPointXPx ist schreibgeschützt, daher können wir ihn nicht direkt setzen.
            // Stattdessen können wir demonstrieren, wie er sich ändert, wenn wir andere Eigenschaften ändern.

            // Ändere den Explosionswert, der die Position des Kuchensegments beeinflusst.
            point.Explosion = 20;
            chart.Calculate(); // Recalculate to update properties

            // Zeige den neuen Wert von ArcStartPointXPx nach der Änderung der Explosion an.
            Console.WriteLine("ArcStartPointXPx after explosion: " + point.ArcStartPointXPx);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointPropertyArcStartPointXPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


