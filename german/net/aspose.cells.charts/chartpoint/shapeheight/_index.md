---
title: "ChartPoint.ShapeHeight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die Höhe in Einheiten von 1/4000 der Diagrammhöhe nach Aufrufen der Methode Chart.Calculate zurück"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/shapeheight/
---
## ChartPoint.ShapeHeight property

Ermittelt die Höhe in Einheiten von 1/4000 der Diagrammhöhe nach Aufrufen der Methode Chart.Calculate().

```csharp
public int ShapeHeight { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightDemo
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
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm berechnen, um sicherzustellen, dass Formeigenschaften verfügbar sind
            chart.Calculate();

            // Den ersten Punkt in der ersten Serie abrufen
            ChartPoint point = chart.NSeries[0].Points[0];

            // Den aktuellen ShapeHeight-Wert anzeigen (in 1/4000 der Diagrammhöhe)
            Console.WriteLine("Current ShapeHeight value: " + point.ShapeHeight);

            // Hinweis: ShapeHeight ist schreibgeschützt, daher können wir ihn nicht direkt setzen
            // Um die Höhe zu ändern, müssen wir die Diagrammgröße oder andere Eigenschaften anpassen

            // Den Effekt demonstrieren, indem die Diagrammhöhe geändert wird
            Console.WriteLine("Original chart height: " + chart.ChartObject.Height);
            chart.ChartObject.Height = 400;
            chart.Calculate(); // Recalculate to update shape properties

            // Den neuen ShapeHeight-Wert nach Änderung der Diagrammhöhe anzeigen
            Console.WriteLine("New ShapeHeight value after chart resize: " + point.ShapeHeight);

            // Ergebnis speichern
            workbook.Save("ChartPointPropertyShapeHeightDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


