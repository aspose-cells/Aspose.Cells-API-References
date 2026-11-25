---
title: "ShapeCollection.AddPictureInChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge un'immagine al grafico."
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addpictureinchart/
---
## ShapeCollection.AddPictureInChart method

Aggiunge un'immagine al grafico.

```csharp
public Picture AddPictureInChart(int top, int left, Stream stream, int widthScale, int heightScale)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| alto | Int32 | Rappresenta lo spostamento verticale della forma dall'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale della forma dall'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |
| stream | Stream | Oggetto Stream che contiene i dati dell'immagine. |
| widthScale | Int32 | Scala della larghezza dell'immagine, in percentuale. |
| heightScale | Int32 | Scala dell'altezza dell'immagine, in percentuale. |

### Valore di ritorno

Restituisce un oggetto Picture.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Crea uno stream di memoria con i dati dell'immagine
            byte[] imageData = File.ReadAllBytes("example.jpg");
            MemoryStream stream = new MemoryStream(imageData);

            try
            {
                // Chiama AddPictureInChart con i parametri (Int32, Int32, Stream, Int32, Int32)
                Picture picture = chart.Shapes.AddPictureInChart(100, 100, stream, 50, 50);
                
                Console.WriteLine("Picture added to chart successfully. Original dimensions: " + 
                    $"{picture.OriginalWidth}x{picture.OriginalHeight}");
                
                // Salva la cartella di lavoro
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

### Vedi anche

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


