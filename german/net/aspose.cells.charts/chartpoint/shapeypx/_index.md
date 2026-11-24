---
title: "ChartPoint.ShapeYPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die y‑Koordinate der oberen linken Ecke in Pixeln zurück, nachdem die Methode Chart.Calculate aufgerufen wurde."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/shapeypx/
---
## ChartPoint.ShapeYPx property

Ermittelt die y‑Koordinate der oberen linken Ecke in Pixeln, nachdem die Methode Chart.Calculate() aufgerufen wurde.

```csharp
public int ShapeYPx { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeYPxDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
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

            // Ersten Punkt in der ersten Serie abrufen
            ChartPoint point = chart.NSeries[0].Points[0];

            // Aktuelle Y‑Position in Pixeln anzeigen
            Console.WriteLine("Current ShapeYPx value: " + point.ShapeYPx);

            // Hinweis: ShapeYPx ist schreibgeschützt, daher kann es nicht direkt gesetzt werden
            // Um die Position zu ändern, müssen wir die Diagrammgröße/-position oder die Daten anpassen

            // Demonstrieren Sie die Wirkung, indem Sie die Diagrammposition ändern, was die Punktpositionen beeinflusst
            chart.Move(2, 3, 17, 11); // Move chart to row 2, column 3
            chart.Calculate(); // Recalculate to update positions

            // Neue Y‑Position nach Diagrammverschiebung anzeigen
            Console.WriteLine("New ShapeYPx value after chart movement: " + point.ShapeYPx);

            // Ergebnis speichern
            workbook.Save("ChartPointShapeYPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


