---
title: "ShapeCollection.AddPictureInChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en bild i diagrammet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addpictureinchart/
---
## ShapeCollection.AddPictureInChart method

Lägger till en bild i diagrammet.

```csharp
public Picture AddPictureInChart(int top, int left, Stream stream, int widthScale, int heightScale)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| top | Int32 | Representerar det vertikala offsetet för formen från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| vänster | Int32 | Representerar det horisontella offsetet för formen från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| ström | Ström | Strömobjekt som innehåller bilddata. |
| widthScale | Int32 | Skala för bildbredd, i procent. |
| heightScale | Int32 | Skala för bildhöjd, i procent. |

### Returvärde

Returnerar ett Picture-objekt.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Skapa en minnesström med bilddata
            byte[] imageData = File.ReadAllBytes("example.jpg");
            MemoryStream stream = new MemoryStream(imageData);

            try
            {
                // Anropa AddPictureInChart med parametrarna (Int32, Int32, Stream, Int32, Int32)
                Picture picture = chart.Shapes.AddPictureInChart(100, 100, stream, 50, 50);
                
                Console.WriteLine("Picture added to chart successfully. Original dimensions: " + 
                    $"{picture.OriginalWidth}x{picture.OriginalHeight}");
                
                // Spara arbetsboken
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

### Se även

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


