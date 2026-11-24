---
title: "ChartPoint.StartAngle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt den Startwinkel für das Kuchensegment zurück, gemessen in Grad im Uhrzeigersinn von der x-Achse nach Aufruf der Chart.Calculate-Methode. Gilt für Kreisdiagramme."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/startangle/
---
## ChartPoint.StartAngle property

Ermittelt den Startwinkel für das Kuchensegment, gemessen in Grad im Uhrzeigersinn von der x‑Achse, nachdem die Methode Chart.Calculate() aufgerufen wurde. Gilt für Kreisdiagramme.

```csharp
public float StartAngle { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyStartAngleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
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
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm berechnen, um sicherzustellen, dass Eigenschaften gefüllt sind.
            chart.Calculate();

            // Den ersten Diagrammpunkt abrufen
            ChartPoint point = chart.NSeries[0].Points[0];

            // Zeige den StartAngle-Wert an.
            Console.WriteLine("StartAngle of first pie slice: " + point.StartAngle);

            // Hinweis: StartAngle ist schreibgeschützt, daher können wir ihn nicht direkt setzen.
            // Um den Startwinkel zu ändern, müssen wir das gesamte Kreisdiagramm drehen.
            chart.NSeries[0].FirstSliceAngle = 90; // Rotate pie chart by 90 degrees

            // Neu berechnen, um die Winkel zu aktualisieren.
            chart.Calculate();

            // Zeige den neuen StartAngle-Wert nach der Drehung an.
            Console.WriteLine("StartAngle after rotation: " + point.StartAngle);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointPropertyStartAngleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


