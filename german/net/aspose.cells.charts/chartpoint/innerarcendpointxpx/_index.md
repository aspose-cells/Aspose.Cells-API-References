---
title: "ChartPoint.InnerArcEndPointXPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die x-Koordinate des Endpunkts des Kuchensegments zurück, nachdem die Methode Chart.Calculate aufgerufen wurde. Gilt für Doughnut-Diagramme"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/innerarcendpointxpx/
---
## ChartPoint.InnerArcEndPointXPx property

Ermittelt die x‑Koordinate des Endpunkts für den Kuchenabschnitt nach Aufruf der Methode Chart.Calculate(). Gilt für Donut‑Diagramme.

```csharp
public float InnerArcEndPointXPx { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcEndPointXPxDemo
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
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(2);

            // Füge ein Doughnut-Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Berechne das Diagramm, um die ChartPoint‑Eigenschaften zu erhalten.
            chart.Calculate();

            // Hole den ersten ChartPoint aus der ersten Serie.
            ChartPoint point = chart.NSeries[0].Points[0];

            // Zeige den aktuellen InnerArcEndPointXPx-Wert
            Console.WriteLine("Current InnerArcEndPointXPx value: " + point.InnerArcEndPointXPx);

            // Hinweis: InnerArcEndPointXPx ist schreibgeschützt, daher können wir ihn nicht direkt setzen
            // Um die Position des Endpunkts zu ändern, müssen wir die Größe des Doughnut-Lochs anpassen
            chart.NSeries[0].DoughnutHoleSize = 50; // Set hole size to 50%

            // Rekalkuliere das Diagramm, um die Eigenschaften zu aktualisieren.
            chart.Calculate();

            // Zeige den neuen InnerArcEndPointXPx-Wert nach Änderung der Lochgröße
            Console.WriteLine("New InnerArcEndPointXPx value after changing doughnut hole size: " + point.InnerArcEndPointXPx);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointPropertyInnerArcEndPointXPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


