---
title: "ChartPoint.ShapeHeightPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die Höhe in Pixeln zurück, nachdem die Methode Chart.Calculate aufgerufen wurde"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/shapeheightpx/
---
## ChartPoint.ShapeHeightPx property

Ermittelt die Höhe in Pixeln nach Aufrufen der Methode Chart.Calculate().

```csharp
public int ShapeHeightPx { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightPxDemo
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

            // Berechnen Sie das Diagramm, um die Formabmessungen zu erhalten
            chart.Calculate();

            // Hole den ersten ChartPoint aus der ersten Serie.
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // Zeigen Sie die aktuelle Höhe der Diagrammpunktform in Pixeln an
            Console.WriteLine("Current ShapeHeightPx value: " + chartPoint.ShapeHeightPx);

            // Hinweis: ShapeHeightPx ist schreibgeschützt, sodass wir ihn nicht direkt setzen können
            // Um die Höhe zu ändern, müssten wir die Diagrammgröße oder die Datenwerte anpassen
            // und das Diagramm neu berechnen

            // Ändern Sie den Datenwert, der die Größe des Diagrammpunkts beeinflusst
            worksheet.Cells["B2"].PutValue(50);
            chart.Calculate();

            // Zeigen Sie die neue Höhe nach Änderung der Daten an
            Console.WriteLine("New ShapeHeightPx value after data change: " + chartPoint.ShapeHeightPx);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointShapeHeightPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


