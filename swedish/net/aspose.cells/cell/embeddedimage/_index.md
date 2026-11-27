---
title: "Cell.EmbeddedImage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Hämtar och sätter den inbäddade bilden i cellen"
type: docs
url: /sv/net/aspose.cells/cell/embeddedimage/
---
## Cell.EmbeddedImage property

Hämtar och anger den inbäddade bilden i cellen.

```csharp
public byte[] EmbeddedImage { get; set; }
```

### Exempel

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
                // Skapa en ny arbetsbok och hämta det första kalkylbladet
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Välj en cell för att lagra den inbäddade bilden
                Cell cell = worksheet.Cells["B2"];

                // En 1x1 pixel transparent PNG (Base64-kodad)
                const string pngBase64 =
                    "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/x8AAwMCAO2b4ZcAAAAASUVORK5CYII=";

                // Konvertera Base64-strängen till en bytearray
                byte[] imageBytes = Convert.FromBase64String(pngBase64);

                // Sätt den inbäddade bilden i cellen
                cell.EmbeddedImage = imageBytes;

                // Hämta den inbäddade bilden tillbaka från cellen
                byte[] retrievedBytes = cell.EmbeddedImage;

                // Skriv den hämtade bilden till en fil för att verifiera att den sparades korrekt
                string outputImagePath = "EmbeddedImage_Output.png";
                File.WriteAllBytes(outputImagePath, retrievedBytes);

                Console.WriteLine($"Embedded image byte length: {retrievedBytes.Length}");
                Console.WriteLine($"Embedded image saved to: {Path.GetFullPath(outputImagePath)}");

                // Spara arbetsboken (den inbäddade bilden lagras i .xlsx-filen)
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

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


