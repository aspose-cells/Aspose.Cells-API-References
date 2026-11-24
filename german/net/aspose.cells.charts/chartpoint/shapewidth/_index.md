---
title: "ChartPoint.ShapeWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die Breite in Einheiten von 1/4000 der Diagrammbreite zurück, nachdem die Methode Chart.Calculate aufgerufen wurde"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/shapewidth/
---
## ChartPoint.ShapeWidth property

Ermittelt die Breite in Einheiten von 1/4000 der Diagrammbreite nach Aufruf der Methode Chart.Calculate().

```csharp
public int ShapeWidth { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeWidthDemo
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
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Diagramm berechnen, um sicherzustellen, dass Formeigenschaften verfügbar sind
            chart.Calculate();
            
            // Den ersten Diagrammpunkt in der ersten Serie abrufen
            ChartPoint point = chart.NSeries[0].Points[0];
            
            // Zeigen Sie den aktuellen Wert von ShapeWidth an (in 1/4000 der Diagrammbreite)
            Console.WriteLine("Current ShapeWidth value: " + point.ShapeWidth);
            
            // Zeigen Sie die Breite in Pixeln an
            Console.WriteLine("Shape width in pixels: " + point.ShapeWidthPx);
            
            // Hinweis: ShapeWidth ist schreibgeschützt, daher können wir es nicht direkt setzen
            // Um die Breite zu ändern, müssten wir die Diagrammgröße oder andere Eigenschaften anpassen
            
            // Ergebnis speichern
            workbook.Save("ChartPointShapeWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


