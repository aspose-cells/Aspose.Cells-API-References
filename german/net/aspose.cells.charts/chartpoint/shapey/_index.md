---
title: "ChartPoint.ShapeY"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die y‑Koordinate der oberen linken Ecke in Einheiten von 1/4000 der Diagrammhöhe zurück, nachdem die Methode Chart.Calculate aufgerufen wurde."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/shapey/
---
## ChartPoint.ShapeY property

Ermittelt die y‑Koordinate der oberen linken Ecke in Einheiten von 1/4000 der Diagrammhöhe nach Aufrufen der Methode Chart.Calculate().

```csharp
public int ShapeY { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeYDemo
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

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm berechnen, um Formpositionen zu erhalten
            chart.Calculate();

            // Den ersten Punkt in der ersten Serie abrufen
            ChartPoint point = chart.NSeries[0].Points[0];

            // Zeige den aktuellen ShapeY‑Wert (1/4000 der Diagrammhöhe) an.
            Console.WriteLine("Current ShapeY value: " + point.ShapeY);

            // Hinweis: ShapeY ist schreibgeschützt, daher können wir ihn nicht direkt setzen.
            // Um die Position zu ändern, müssten wir die zugrunde liegenden Daten oder Diagrammeigenschaften anpassen.

            // Demonstriere, wie ShapeY mit der tatsächlichen Position zusammenhängt.
            Console.WriteLine("ShapeY in pixels: " + point.ShapeYPx);
            Console.WriteLine("Chart height in pixels: " + (point.ShapeYPx * 4000 / point.ShapeY));

            // Ergebnis speichern
            workbook.Save("ChartPointPropertyShapeYDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


