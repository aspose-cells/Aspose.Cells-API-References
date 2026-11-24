---
title: "Series.Move"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Methode. Verschiebt die Serie nach oben oder unten"
type: docs
url: /de/net/aspose.cells.charts/series/move/
---
## Series.Move method

Verschiebt die Serie nach oben oder unten.

```csharp
public void Move(int count)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Anzahl | Int32 | Die Anzahl der Verschiebungen nach oben oder unten. Verschiebe die Serie nach oben, wenn dieser Wert kleiner als Null ist; verschiebe die Serie nach unten, wenn dieser Wert größer als Null ist. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesMethodMoveWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Serie zum Diagramm hinzufügen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Erhalte die erste Serie
            Series series = chart.NSeries[0];
            
            try
            {
                // Rufen Sie die Move-Methode mit einem Int32-Parameter auf
                series.Move(1);
                
                Console.WriteLine("Series moved successfully by 1 position");
                
                // Zeigen Sie die Wirkung, indem Sie den Seriennamen ändern
                series.Name = "Moved Series";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("SeriesMethodMoveWithInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


