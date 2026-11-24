---
title: "ChartPoint.ArcEndPointXPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die x-Koordinate des Endpunkts des Kuchensegments zurück, nachdem die Methode Chart.Calculate aufgerufen wurde. Gilt für Pie- und Doughnut-Diagramme"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/arcendpointxpx/
---
## ChartPoint.ArcEndPointXPx property

Ermittelt die x‑Koordinate des Endpunkts des Kuchensegments nach Aufruf der Methode Chart.Calculate(). Gilt für Kreis‑ und Donut‑Diagramme.

```csharp
public float ArcEndPointXPx { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcEndPointXPxDemo
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
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Ein Kreisdiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm berechnen, um sicherzustellen, dass Eigenschaften gefüllt sind.
            chart.Calculate();

            // Den ersten Diagrammpunkt abrufen
            ChartPoint point = chart.NSeries[0].Points[0];

            // Zeige den ArcEndPointXPx-Wert
            Console.WriteLine("ArcEndPointXPx: " + point.ArcEndPointXPx);

            // Hinweis: ArcEndPointXPx ist schreibgeschützt, daher können wir ihn nicht direkt setzen
            // Um den Endpunkt zu ändern, müssen wir die Diagrammdaten oder Eigenschaften anpassen, die das Kuchensegment beeinflussen
            
            // Beispiel dafür, wie das Ändern von Daten den ArcEndPointXPx beeinflusst
            worksheet.Cells["B2"].PutValue(60); // Increase Apple's value
            chart.Calculate(); // Recalculate chart

            // Zeige den neuen ArcEndPointXPx-Wert nach Datenänderung
            Console.WriteLine("New ArcEndPointXPx after data change: " + point.ArcEndPointXPx);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointPropertyArcEndPointXPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


