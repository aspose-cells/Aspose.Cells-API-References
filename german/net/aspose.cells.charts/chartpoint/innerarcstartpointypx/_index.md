---
title: "ChartPoint.InnerArcStartPointYPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die Y‑Koordinate des Startpunkts des Kuchenabschnitts zurück, nachdem die Methode Chart.Calculate aufgerufen wurde. Gilt für Doughnut‑Diagramme."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/innerarcstartpointypx/
---
## ChartPoint.InnerArcStartPointYPx property

Ermittelt die y‑Koordinate des Startpunkts für den Kuchenabschnitt nach Aufrufen der Methode Chart.Calculate(). Gilt für Donut‑Diagramm.

```csharp
public float InnerArcStartPointYPx { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcStartPointYPxDemo
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
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm berechnen, um sicherzustellen, dass Eigenschaften gefüllt sind.
            chart.Calculate();

            // Den ersten Diagrammpunkt abrufen
            ChartPoint point = chart.NSeries[0].Points[0];

            // Zeige den InnerArcStartPointYPx‑Wert an.
            Console.WriteLine("InnerArcStartPointYPx: " + point.InnerArcStartPointYPx);

            // Hinweis: InnerArcStartPointYPx ist schreibgeschützt, daher können wir ihn nicht direkt setzen.
            // Um die Position zu ändern, müssen wir die Größe des Doughnut‑Lochs anpassen.
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // Rekalkuliere das Diagramm, um die Eigenschaften zu aktualisieren.
            chart.Calculate();

            // Zeige den neuen InnerArcStartPointYPx‑Wert nach Änderung der Lochgröße an.
            Console.WriteLine("New InnerArcStartPointYPx after changing hole size: " + point.InnerArcStartPointYPx);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointPropertyInnerArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


