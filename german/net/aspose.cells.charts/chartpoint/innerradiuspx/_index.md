---
title: "ChartPoint.InnerRadiusPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt den inneren Radius eines Donut-Segments in Pixeln nach Aufrufen der Methode Chart.Calculate zurück. Gilt für Donut-Diagramme"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/innerradiuspx/
---
## ChartPoint.InnerRadiusPx property

Gibt den inneren Radius eines Donut-Segments in Pixeln nach Aufrufen der Methode Chart.Calculate() zurück. Gilt für Donut-Diagramme.

```csharp
[Obsolete("Use ChartPoint.DoughnutInnerRadius property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerRadiusPx { get; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft ChartPoint.DoughnutInnerRadius. Diese Eigenschaft wird 12 Monate nach Juni 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerRadiusPxDemo
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
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(5);

            // Füge ein Doughnut-Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm berechnen, um die ChartPoint-Eigenschaften zu erhalten
            chart.Calculate();

            // Hole den ersten ChartPoint aus der ersten Serie.
            ChartPoint point = chart.NSeries[0].Points[0];

            // Den aktuellen inneren Radiuswert anzeigen (schreibgeschützte Eigenschaft)
            Console.WriteLine("Current InnerRadiusPx value: " + point.InnerRadiusPx);

            // Hinweis: InnerRadiusPx ist schreibgeschützt, daher können wir ihn nicht direkt setzen
            // Um den inneren Radius zu ändern, müssen wir die Größe des Donut-Lochs anpassen
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // Rekalkuliere das Diagramm, um die Eigenschaften zu aktualisieren.
            chart.Calculate();

            // Den neuen inneren Radiuswert nach Änderung der Donut-Lochgröße anzeigen
            Console.WriteLine("New InnerRadiusPx value after changing DoughnutHoleSize: " + point.InnerRadiusPx);

            // Ergebnis speichern
            workbook.Save("ChartPointPropertyInnerRadiusPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


