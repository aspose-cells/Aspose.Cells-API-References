---
title: "ChartPoint.ShapeWidthPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die Breite in Pixeln zurück, nachdem die Methode Chart.Calculate aufgerufen wurde"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/shapewidthpx/
---
## ChartPoint.ShapeWidthPx property

Ermittelt die Breite in Pixeln nach Aufruf der Methode Chart.Calculate().

```csharp
public int ShapeWidthPx { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeWidthPxDemo
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

            // Diagramm berechnen, um sicherzustellen, dass Formeigenschaften verfügbar sind
            chart.Calculate();

            // Hole den ersten Diagrammpunkt aus der ersten Serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Zeigen Sie die aktuelle Breite der Diagrammpunktform in Pixeln an
            Console.WriteLine("Current ShapeWidthPx value: " + point.ShapeWidthPx);

            // Hinweis: ShapeWidthPx ist schreibgeschützt, daher können wir es nicht direkt setzen
            // Um die Breite zu ändern, müssen wir die Größe des Diagramms oder andere Eigenschaften anpassen
            // dies würde die Breite des Punktes bei der nächsten Berechnung (Calculate) beeinflussen

            // Ändern Sie die Breite des Diagramms, um zu demonstrieren, wie sie ShapeWidthPx beeinflusst
            chart.ChartObject.Width = 1000;
            chart.Calculate();

            // Zeigen Sie die neue Breite nach der Diagrammgrößeänderung an
            Console.WriteLine("New ShapeWidthPx value after chart resize: " + point.ShapeWidthPx);

            // Ergebnis speichern
            workbook.Save("ChartPointPropertyShapeWidthPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


