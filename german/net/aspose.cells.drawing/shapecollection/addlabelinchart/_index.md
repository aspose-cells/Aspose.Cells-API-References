---
title: "ShapeCollection.AddLabelInChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein Label zur Grafik hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addlabelinchart/
---
## ShapeCollection.AddLabelInChart method

Fügt ein Label zum Diagramm hinzu.

```csharp
public Label AddLabelInChart(int top, int left, int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oben | Int32 | Stellt den vertikalen Versatz des Labels von der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs dar. |
| links | Int32 | Stellt den vertikalen Versatz des Labels von der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs dar. |
| Höhe | Int32 | Stellt die Höhe des Labels in Einheiten von 1/4000 des Diagrammbereichs dar. |
| Breite | Int32 | Stellt die Breite des Labels in Einheiten von 1/4000 des Diagrammbereichs dar. |

### Rückgabewert

Ein neues Label-Objekt.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten hinzufügen, um ein Diagramm zu erstellen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];            
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Rufen Sie die Methode AddLabelInChart mit den Parametern (top, left, height, width) auf
                Label label = chart.Shapes.AddLabelInChart(100, 100, 200, 200);
                
                // Label-Eigenschaften festlegen
                label.Text = "Sample Chart Label";
                label.Font.Color = System.Drawing.Color.Red;
                label.Font.Size = 12;

                Console.WriteLine("Label added successfully to chart with parameters (100, 100, 200, 50)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddLabelInChart method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


