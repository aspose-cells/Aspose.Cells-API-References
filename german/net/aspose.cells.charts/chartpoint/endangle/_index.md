---
title: "ChartPoint.EndAngle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt den Endwinkel für das Kuchensegment zurück, gemessen in Grad im Uhrzeigersinn von der x‑Achse nach Aufruf der Methode Chart.Calculate. Gilt für Kreis‑Diagramme."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/endangle/
---
## ChartPoint.EndAngle property

Ermittelt den Endwinkel für den Kuchenabschnitt, gemessen in Grad im Uhrzeigersinn von der x‑Achse nach Aufrufen der Methode Chart.Calculate(). Gilt für Kreis‑Diagramm.

```csharp
public float EndAngle { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyEndAngleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für das Kreisdiagramm hinzu.
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Ein Kreisdiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm berechnen, um sicherzustellen, dass Eigenschaften gefüllt sind.
            chart.Calculate();

            // Hole den ersten Diagrammpunkt (Apfel‑Segment).
            ChartPoint point = chart.NSeries[0].Points[0];

            // Zeige den aktuellen EndAngle‑Wert an.
            Console.WriteLine("Current EndAngle value: " + point.EndAngle);

            // Hinweis: EndAngle ist schreibgeschützt, daher können wir ihn nicht direkt setzen.
            // Stattdessen zeigen wir, wie er sich auf das Kuchensegment bezieht.

            // Explodiere den Punkt, um zu sehen, wie er die Winkel beeinflusst.
            point.Explosion = 20;
            chart.Calculate(); // Recalculate to update angles

            // Zeige den neuen EndAngle nach der Explosion an.
            Console.WriteLine("EndAngle after explosion: " + point.EndAngle);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointEndAngleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


