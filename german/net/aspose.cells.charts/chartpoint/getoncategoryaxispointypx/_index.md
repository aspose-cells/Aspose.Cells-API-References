---
title: "ChartPoint.GetOnCategoryAxisPointYPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Methode. Gibt die y-Koordinate des Punktes auf der Kategorienachse zurück, nachdem die Methode Chart.Calculate aufgerufen wurde. Gilt nur für das Area-Diagramm"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/getoncategoryaxispointypx/
---
## ChartPoint.GetOnCategoryAxisPointYPx method

Ermittelt die y‑Koordinate des Punktes auf der Kategorienachse, nachdem die Methode Chart.Calculate() aufgerufen wurde. Gilt nur für Flächendiagramme.

```csharp
public float GetOnCategoryAxisPointYPx(int index)
```

### Hinweise

2D-Flächendiagramm: Index ist 0. 3D-Flächendiagramm: Index ist 0 oder 1.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetOnCategoryAxisPointYPxWithInt32Demo
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

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Berechne das Diagramm, um sicherzustellen, dass alle Positions-Eigenschaften berechnet werden
            chart.Calculate();

            // Hole den ersten Diagrammpunkt aus der ersten Serie
            ChartPoint point = chart.NSeries[0].Points[0];

            try
            {
                // Rufe GetOnCategoryAxisPointYPx mit Index 0 auf
                float yPx = point.GetOnCategoryAxisPointYPx(0);
                
                // Ergebnis anzeigen
                Console.WriteLine($"Y coordinate of point on category axis: {yPx} pixels");
                
                // Speichere die Arbeitsmappe
                workbook.Save("ChartPointGetOnCategoryAxisPointYPxDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointYPx method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


