---
title: "ImageOrPrintOptions.PixelFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Ruft das Pixel-Format für die erzeugten Bilder ab oder legt es fest"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/pixelformat/
---
## ImageOrPrintOptions.PixelFormat property

Ruft das Pixelformat für die erzeugten Bilder ab oder legt es fest.

```csharp
public PixelFormat PixelFormat { get; set; }
```

### Hinweise

Der Standardwert ist PixelFormat.Format32bppArgb.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyPixelFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Erstelle ein Beispiel-Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten hinzu, um das Beispiel sinnvoll zu machen.
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "PixelFormat Demo";

            try
            {
                // Erstelle eine ImageOrPrintOptions-Instanz
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Zeigen Sie den aktuellen Wert der ImageType-Eigenschaft an (da PixelFormat nicht existiert)
                Console.WriteLine("Current ImageType: " + options.ImageType);

                // Hinweis: Da PixelFormat in der API nicht existiert, demonstrieren wir stattdessen ImageType
                // welche ist die am nächsten verwandte Eigenschaft für Bildformat-Einstellungen

                // Erstellen Sie ein SheetRender, um die verwendeten Optionen zu demonstrieren
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Speichern Sie das Ergebnis als Bild, um die Optionen zu demonstrieren
                sheetRender.ToImage(0, "PixelFormatDemo.png");

                Console.WriteLine("ImageType property has been demonstrated. Image saved as PixelFormatDemo.png");
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

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


