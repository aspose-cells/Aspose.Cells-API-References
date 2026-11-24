---
title: "ChartPoint.ShapeXPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die x‑Koordinate der oberen linken Ecke in Pixeln zurück, nach Aufruf der Chart.Calculate‑Methode."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/shapexpx/
---
## ChartPoint.ShapeXPx property

Ermittelt die x‑Koordinate der oberen linken Ecke in Pixeln nach Aufruf der Methode Chart.Calculate().

```csharp
public int ShapeXPx { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeXPxDemo
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

            // Berechne das Diagramm, um die Formpositionen zu erhalten.
            chart.Calculate();

            // Hole den ersten ChartPoint aus der ersten Serie.
            ChartPoint point = chart.NSeries[0].Points[0];

            // Zeige die aktuelle X‑Position in Pixeln an.
            Console.WriteLine("Current ShapeXPx value: " + point.ShapeXPx);

            // Hinweis: ShapeXPx ist schreibgeschützt, daher können wir es nicht direkt setzen.
            // Um die Position zu ändern, müssten wir die Diagrammgröße/‑position oder die Daten anpassen.

            // Demonstriere, wie sich die Eigenschaft ändert, wenn wir das Diagramm modifizieren.
            Console.WriteLine("\nChanging chart position...");
            chart.ChartObject.Left = 3;
            chart.ChartObject.Top = 2;
            chart.Calculate(); // Recalculate to update positions

            Console.WriteLine("New ShapeXPx value after chart move: " + point.ShapeXPx);

            // Ergebnis speichern
            workbook.Save("ChartPointPropertyShapeXPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


