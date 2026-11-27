---
title: "Enum ImageBinarizationMethod"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.ImageBinarizationMethod enum. Anger metoden som används för att binarisera bilden"
type: docs
url: /sv/net/aspose.cells.rendering/imagebinarizationmethod/
---
## ImageBinarizationMethod enumeration

Specificerar metoden som används för att binarisera bild.

```csharp
public enum ImageBinarizationMethod
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Threshold | `0` | Anger tröskelmetod. |
| FloydSteinbergDithering | `1` | Anger dithering med Floyd‑Steinberg felspredningsmetod. |

### Exempel

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
            // Skapa en ny arbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll celler med gradientvärden för demonstration
            for (int row = 0; row < 50; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue((double)(row * col) / 500);
                }
            }

            // Konfigurera bildrenderingsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT4,
                TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering
            };

            // Skapa bladrendering med konfigurerade alternativ
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // Rendera första arbetsbladssidan till bild med binarisering
            renderer.ToImage(0, "BinarizedOutput.tiff");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


