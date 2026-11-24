---
title: "ChartPoint.InnerArcEndPointYPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die Y‑Koordinate des Endpunkts des Kuchenabschnitts zurück, nachdem die Methode Chart.Calculate aufgerufen wurde. Gilt für Doughnut‑Diagramme."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/innerarcendpointypx/
---
## ChartPoint.InnerArcEndPointYPx property

Ermittelt die y‑Koordinate des Endpunkts für den Kuchenabschnitt nach Aufrufen der Methode Chart.Calculate(). Gilt für Donut‑Diagramm.

```csharp
public float InnerArcEndPointYPx { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcEndPointYPxDemo
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
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["B3"].PutValue(35);
            worksheet.Cells["B4"].PutValue(25);

            // Füge ein Doughnut-Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Berechne das Diagramm, um die ChartPoint‑Eigenschaften zu erhalten.
            chart.Calculate();

            // Hole den ersten ChartPoint aus der ersten Serie.
            ChartPoint point = chart.NSeries[0].Points[0];

            // Zeige den aktuellen InnerArcEndPointYPx‑Wert an.
            Console.WriteLine("Current InnerArcEndPointYPx value: " + point.InnerArcEndPointYPx);

            // Hinweis: InnerArcEndPointYPx ist schreibgeschützt, daher können wir ihn nicht direkt setzen.
            // Um die Position zu ändern, müssen wir die Größe des Doughnut‑Lochs anpassen.
            chart.NSeries[0].DoughnutHoleSize = 60; // Change hole size to affect inner arc position

            // Rekalkuliere das Diagramm, um die Eigenschaften zu aktualisieren.
            chart.Calculate();

            // Zeige den neuen InnerArcEndPointYPx‑Wert nach Änderung der Lochgröße an.
            Console.WriteLine("New InnerArcEndPointYPx value after changing hole size: " + point.InnerArcEndPointYPx);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointPropertyInnerArcEndPointYPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


