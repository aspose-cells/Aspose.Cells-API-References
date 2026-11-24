---
title: "Enum ImageBinarizationMethod"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.ImageBinarizationMethod enum. Gibt die Methode an, die zum Binarisieren von Bildern verwendet wird."
type: docs
url: /de/net/aspose.cells.rendering/imagebinarizationmethod/
---
## ImageBinarizationMethod enumeration

Gibt die Methode an, die zum Binarisieren von Bildern verwendet wird.

```csharp
public enum ImageBinarizationMethod
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Threshold | `0` | Gibt die Schwellenwertmethode an. |
| FloydSteinbergDithering | `1` | Gibt das Dithering mit der Floyd‑Steinberg-Fehlerdiffusionsmethode an. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class RenderingClassImageBinarizationMethodDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe mit Testdaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füllen Sie Zellen mit Gradientenwerten zur Demonstration
            for (int row = 0; row < 50; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue((double)(row * col) / 500);
                }
            }

            // Konfigurieren Sie die Bildrenderoptionen
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT4,
                TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering
            };

            // Erstellen Sie ein Blatt-Rendering mit den konfigurierten Optionen
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // Rendern Sie die erste Arbeitsblattseite als Bild mit Binarisierung
            renderer.ToImage(0, "BinarizedOutput.tiff");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


