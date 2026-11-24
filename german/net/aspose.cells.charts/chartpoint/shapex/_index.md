---
title: "ChartPoint.ShapeX"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die x‑Koordinate der oberen linken Ecke in Einheiten von 1/4000 der Diagrammbreite zurück, nachdem die Methode Chart.Calculate aufgerufen wurde."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/shapex/
---
## ChartPoint.ShapeX property

Ermittelt die x‑Koordinate der oberen linken Ecke in Einheiten von 1/4000 der Diagrammbreite nach Aufruf der Methode Chart.Calculate().

```csharp
public int ShapeX { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeXDemo
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

            // Berechne das Diagramm, um sicherzustellen, dass ShapeX gefüllt ist.
            chart.Calculate();

            // Den ersten Punkt in der ersten Serie abrufen
            ChartPoint point = chart.NSeries[0].Points[0];

            // Zeige den ShapeX‑Wert (1/4000 der Diagrammbreite) an.
            Console.WriteLine("ShapeX value (1/4000 units): " + point.ShapeX);
            Console.WriteLine("ShapeX value (pixels): " + point.ShapeXPx);

            // Demonstriere die Verwendung von ShapeX, um Elemente relativ zum Diagrammpunkt zu positionieren.
            // Hinweis: Da ShapeX schreibgeschützt ist, können wir ihn nicht direkt ändern,
            // aber wir können ihn verwenden, um andere Elemente zu positionieren.
            if (point.ShapeX > 0)
            {
                // Füge ein Textfeld hinzu, das mit der X‑Position des Diagrammpunkts ausgerichtet ist.
                Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(
                    point.ShapeXPx, 100, 100, 50, 100, 50);
                textBox.Text = "Point 1";
            }

            // Ergebnis speichern
            workbook.Save("ChartPointShapeXDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


