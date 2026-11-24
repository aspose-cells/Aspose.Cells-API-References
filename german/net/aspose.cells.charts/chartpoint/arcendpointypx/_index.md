---
title: "ChartPoint.ArcEndPointYPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die y-Koordinate des Endpunkts für das Kuchensegment nach Aufrufen der Methode Chart.Calculate zurück. Gilt für Kreis- und Donut-Diagramme"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/arcendpointypx/
---
## ChartPoint.ArcEndPointYPx property

Ermittelt die y‑Koordinate des Endpunkts des Kuchensegments nach Aufruf der Methode Chart.Calculate(). Gilt für Kreis‑ und Donut‑Diagramme.

```csharp
public float ArcEndPointYPx { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcEndPointYPxDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("C1");
            worksheet.Cells["A3"].PutValue("C2");
            worksheet.Cells["A4"].PutValue("C3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(8000);
            worksheet.Cells["B3"].PutValue(12000);
            worksheet.Cells["B4"].PutValue(14000);

            // Ein Kreisdiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm berechnen, um die Formpositionen zu erhalten
            chart.Calculate();

            // Den ersten Diagrammpunkt abrufen
            ChartPoint point = chart.NSeries[0].Points[0];

            // Den aktuellen ArcEndPointYPx-Wert anzeigen
            Console.WriteLine("Current ArcEndPointYPx value: " + point.ArcEndPointYPx);

            // Da ArcEndPointYPx schreibgeschützt ist, können wir ihn nur lesen
            // Die folgende Zeile würde einen Kompilierungsfehler verursachen:
            // point.ArcEndPointYPx = 150.5f;

            // Demonstrieren, wie diese Eigenschaft das Kuchendiagramm beeinflusst
            Console.WriteLine("Pie slice end point Y coordinate: " + point.ArcEndPointYPx + " pixels");

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointPropertyArcEndPointYPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


