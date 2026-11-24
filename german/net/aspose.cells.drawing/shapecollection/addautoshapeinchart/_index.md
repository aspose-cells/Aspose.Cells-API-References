---
title: "ShapeCollection.AddAutoShapeInChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein AutoShape zum Diagramm hinzu."
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addautoshapeinchart/
---
## ShapeCollection.AddAutoShapeInChart method

Fügt ein AutoShape zum Diagramm hinzu.

```csharp
public Shape AddAutoShapeInChart(AutoShapeType type, int top, int left, int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | AutoShapeType | Auto-Formtyp. |
| oben | Int32 | Stellt den vertikalen Versatz des Textfelds von der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs dar. |
| links | Int32 | Stellt den vertikalen Versatz des Textfelds von der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs dar. |
| Höhe | Int32 | Stellt die Höhe des Textfelds in Einheiten von 1/4000 des Diagrammbereichs dar. |
| Breite | Int32 | Stellt die Breite des Textfelds in Einheiten von 1/4000 des Diagrammbereichs dar. |

### Rückgabewert

Gibt ein Formobjekt zurück.

### Hinweise

Der Typ darf nicht Chart/Comment/Picture/OleObject/Polygon/DialogBox sein

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddAutoShapeInChartWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Rufen Sie die Methode AddAutoShapeInChart auf, um eine Sternform zum Diagramm hinzuzufügen.
                Shape shape = chart.Shapes.AddAutoShapeInChart(
                    AutoShapeType.Star16,  // AutoShapeType
                    100,                  // Top position (in pixels)
                    100,                  // Left position (in pixels)
                    200,                  // Height (in pixels)
                    200);                 // Width (in pixels)

                // Formeigenschaften festlegen
                shape.Name = "SampleStar";
                shape.Fill.SolidFill.Color = System.Drawing.Color.Yellow;
                shape.Line.SolidFill.Color = System.Drawing.Color.Red;

                Console.WriteLine("Star shape added successfully to the chart.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAutoShapeInChart method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("ShapeCollectionMethodAddAutoShapeInChartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


