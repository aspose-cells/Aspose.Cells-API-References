---
title: "ShapeCollection.AddPictureInChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein Bild zum Diagramm hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addpictureinchart/
---
## ShapeCollection.AddPictureInChart method

Fügt ein Bild zum Diagramm hinzu.

```csharp
public Picture AddPictureInChart(int top, int left, Stream stream, int widthScale, int heightScale)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oben | Int32 | Stellt den vertikalen Versatz der Form vom oberen linken Eckpunkt in Einheiten von 1/4000 des Diagrammbereichs dar. |
| links | Int32 | Stellt den horizontalen Versatz der Form vom oberen linken Eckpunkt in Einheiten von 1/4000 des Diagrammbereichs dar. |
| Stream | Stream | Stream-Objekt, das die Bilddaten enthält. |
| widthScale | Int32 | Skalierung der Bildbreite, ein Prozentsatz. |
| heightScale | Int32 | Skalierung der Bildhöhe, ein Prozentsatz. |

### Rückgabewert

Gibt ein Picture-Objekt zurück.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts; // Added this using directive
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ShapeCollectionMethodAddPictureInChartWithInt32Int32StreamInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Erstelle einen Memory-Stream mit Bilddaten
            byte[] imageData = File.ReadAllBytes("example.jpg");
            MemoryStream stream = new MemoryStream(imageData);

            try
            {
                // Rufe AddPictureInChart mit den Parametern (Int32, Int32, Stream, Int32, Int32) auf
                Picture picture = chart.Shapes.AddPictureInChart(100, 100, stream, 50, 50);
                
                Console.WriteLine("Picture added to chart successfully. Original dimensions: " + 
                    $"{picture.OriginalWidth}x{picture.OriginalHeight}");
                
                // Speichere die Arbeitsmappe
                workbook.Save("AddPictureInChartDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPictureInChart method: {ex.Message}");
            }
            finally
            {
                stream.Dispose();
            }
        }
    }
}
```

### Siehe auch

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


