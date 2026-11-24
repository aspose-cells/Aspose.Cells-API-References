---
title: "ChartPoint.InnerArcStartPointXPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die x-Koordinate des Startpunkts des Kuchensegments zurück, nachdem die Methode Chart.Calculate aufgerufen wurde. Gilt für das Doughnut-Diagramm"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/innerarcstartpointxpx/
---
## ChartPoint.InnerArcStartPointXPx property

Ermittelt die x‑Koordinate des Startpunkts für den Kuchenabschnitt nach Aufruf der Methode Chart.Calculate(). Gilt für das Donut‑Diagramm.

```csharp
public float InnerArcStartPointXPx { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcStartPointXPxDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Doughnut-Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Berechne das Diagramm, um die Formeigenschaften zu erhalten
            chart.Calculate();

            // Den ersten Diagrammpunkt abrufen
            ChartPoint point = chart.NSeries[0].Points[0];

            // Anzeige des InnerArcStartPointXPx-Werts
            Console.WriteLine("InnerArcStartPointXPx: " + point.InnerArcStartPointXPx);

            // Hinweis: InnerArcStartPointXPx ist schreibgeschützt, daher können wir ihn nicht direkt setzen
            // Um die Position zu ändern, müssten wir die Diagrammgröße oder die Größe des Doughnut-Lochs anpassen

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointPropertyInnerArcStartPointXPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


