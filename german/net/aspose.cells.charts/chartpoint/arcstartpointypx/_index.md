---
title: "ChartPoint.ArcStartPointYPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die y‑Koordinate des Startpunkts für das Kuchensegment zurück, nachdem die Methode Chart.Calculate aufgerufen wurde. Gilt für Kreis‑ und Donut‑Diagramme."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/arcstartpointypx/
---
## ChartPoint.ArcStartPointYPx property

Ermittelt die y‑Koordinate des Startpunkts für den Kuchenabschnitt nach Aufrufen der Methode Chart.Calculate(). Gilt für Kreis‑ und Donut‑Diagramme.

```csharp
public float ArcStartPointYPx { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcStartPointYPxDemo
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

            // Ein Kreisdiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm berechnen, um die Formpositionen zu erhalten
            chart.Calculate();

            // Den ersten Diagrammpunkt abrufen
            ChartPoint point = chart.NSeries[0].Points[0];

            // Zeige den aktuellen Wert von ArcStartPointYPx an.
            Console.WriteLine("Current ArcStartPointYPx value: " + point.ArcStartPointYPx);

            // Hinweis: ArcStartPointYPx ist schreibgeschützt, sodass wir ihn nicht direkt setzen können
            // Stattdessen zeigen wir, wie das Ändern anderer Eigenschaften ArcStartPointYPx beeinflusst

            // Ändern Sie den Explosionswert, um die Position des Kuchensegments zu ändern
            point.Explosion = 20;

            // Rechnen Sie das Diagramm neu, um die Positionen zu aktualisieren
            chart.Calculate();

            // Zeigen Sie den neuen ArcStartPointYPx-Wert nach Änderung der Explosion an
            Console.WriteLine("New ArcStartPointYPx after explosion change: " + point.ArcStartPointYPx);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointPropertyArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


