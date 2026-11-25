---
title: "Cell.EmbeddedImage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Cell proprietà. Ottiene e imposta l'immagine incorporata nella cella"
type: docs
url: /it/net/aspose.cells/cell/embeddedimage/
---
## Cell.EmbeddedImage property

Restituisce e imposta l'immagine incorporata nella cella.

```csharp
public byte[] EmbeddedImage { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellPropertyEmbeddedImageDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Scegli una cella per memorizzare l'immagine incorporata
                Cell cell = worksheet.Cells["B2"];

                // Un PNG trasparente 1x1 pixel (codificato Base64)
                const string pngBase64 =
                    "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/x8AAwMCAO2b4ZcAAAAASUVORK5CYII=";

                // Converti la stringa Base64 in un array di byte
                byte[] imageBytes = Convert.FromBase64String(pngBase64);

                // Imposta l'immagine incorporata nella cella
                cell.EmbeddedImage = imageBytes;

                // Recupera l'immagine incorporata dalla cella
                byte[] retrievedBytes = cell.EmbeddedImage;

                // Scrivi l'immagine recuperata su un file per verificare che sia stata memorizzata correttamente
                string outputImagePath = "EmbeddedImage_Output.png";
                File.WriteAllBytes(outputImagePath, retrievedBytes);

                Console.WriteLine($"Embedded image byte length: {retrievedBytes.Length}");
                Console.WriteLine($"Embedded image saved to: {Path.GetFullPath(outputImagePath)}");

                // Salva la cartella di lavoro (l'immagine incorporata è memorizzata all'interno del .xlsx)
                string workbookPath = "EmbeddedImageDemo.xlsx";
                workbook.Save(workbookPath);
                Console.WriteLine($"Workbook saved to: {Path.GetFullPath(workbookPath)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


