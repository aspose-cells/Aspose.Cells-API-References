---
title: "MsoFillFormatHelper.ImageData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFillFormatHelper property. Liest und schreibt die Textur- und Bildfüllungsdaten"
type: docs
url: /de/net/aspose.cells.drawing/msofillformathelper/imagedata/
---
## MsoFillFormatHelper.ImageData property

Liest und setzt die Textur- und Bildfüllungsdaten.

```csharp
public byte[] ImageData { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;
    using System.IO;

    public class MsoFillFormatHelperPropertyImageDataDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Label hinzu, um das Beispiel sinnvoll zu machen
            worksheet.Cells["A1"].Value = "ImageData Property Demo";

            try
            {
                // Erstelle eine Instanz von MsoFillFormatHelper mittels Reflexion (kein öffentlicher Konstruktor)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Zeige den aktuellen Wert der ImageData-Eigenschaft an
                Console.WriteLine($"Current ImageData: {(fillHelper.ImageData == null ? "null" : $"Length: {fillHelper.ImageData.Length} bytes")}");

                // Setze neue Bilddaten (erstelle ein einfaches 1x1-Pixel-rotes Bild)
                byte[] imageData = new byte[] { 0x42, 0x4D, 0x3A, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00, 0x28, 0x00,
                                               0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x18, 0x00, 0x00, 0x00,
                                               0x00, 0x00, 0x04, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                                               0x00, 0x00, 0x00, 0x00, 0x00, 0xFF, 0x00, 0x00 };

                fillHelper.ImageData = imageData;
                Console.WriteLine($"Updated ImageData length: {fillHelper.ImageData.Length} bytes");

                // Demonstriere das Auslesen des ImageData-Werts
                byte[] currentImageData = fillHelper.ImageData;
                Console.WriteLine($"Current ImageData length: {currentImageData.Length} bytes");

                // Speichern Sie die Arbeitsmappe, um die erfolgreiche Ausführung zu demonstrieren
                workbook.Save("ImageDataDemo.xlsx");

                Console.WriteLine("ImageData property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ImageData demo: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


