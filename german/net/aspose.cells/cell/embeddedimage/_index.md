---
title: "Cell.EmbeddedImage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt das eingebettete Bild in der Zelle zurück und setzt es"
type: docs
url: /de/net/aspose.cells/cell/embeddedimage/
---
## Cell.EmbeddedImage property

Liefert und setzt das eingebettete Bild in der Zelle.

```csharp
public byte[] EmbeddedImage { get; set; }
```

### Beispiele

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
                // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Wählen Sie eine Zelle aus, um das eingebettete Bild zu speichern
                Cell cell = worksheet.Cells["B2"];

                // Ein 1x1 Pixel transparentes PNG (Base64-kodiert)
                const string pngBase64 =
                    "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/x8AAwMCAO2b4ZcAAAAASUVORK5CYII=";

                // Konvertieren Sie die Base64-Zeichenkette in ein Byte-Array
                byte[] imageBytes = Convert.FromBase64String(pngBase64);

                // Legen Sie das eingebettete Bild in die Zelle
                cell.EmbeddedImage = imageBytes;

                // Rufen Sie das eingebettete Bild aus der Zelle ab
                byte[] retrievedBytes = cell.EmbeddedImage;

                // Schreiben Sie das abgerufene Bild in eine Datei, um zu überprüfen, ob es korrekt gespeichert wurde
                string outputImagePath = "EmbeddedImage_Output.png";
                File.WriteAllBytes(outputImagePath, retrievedBytes);

                Console.WriteLine($"Embedded image byte length: {retrievedBytes.Length}");
                Console.WriteLine($"Embedded image saved to: {Path.GetFullPath(outputImagePath)}");

                // Speichern Sie die Arbeitsmappe (das eingebettete Bild wird in der .xlsx gespeichert)
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

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


