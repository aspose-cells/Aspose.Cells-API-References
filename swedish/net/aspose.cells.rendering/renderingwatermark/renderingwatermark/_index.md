---
title: "RenderingWatermark.RenderingWatermark"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingWatermark-konstruktör. Skapar en instans av textvattenstämpel"
type: docs
url: /sv/net/aspose.cells.rendering/renderingwatermark/renderingwatermark/
---
## RenderingWatermark(string, RenderingFont) {#constructor_1}

Skapar en instans av textvattenstämpel.

```csharp
public RenderingWatermark(string text, RenderingFont renderingFont)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | String | vattenstämpeltext |
| renderingFont | RenderingFont | vattenstämpelfont |

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkMethodCtorWithStringRenderingFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa ett RenderingFont‑objekt
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Color = Color.Blue
            };

            // Skapa ett RenderingWatermark-objekt med hjälp av #ctor(string, RenderingFont)
            RenderingWatermark watermark = new RenderingWatermark("DEMO WATERMARK", renderingFont)
            {
                Rotation = 45,
                Opacity = 0.3f
            };

            // Skapa PdfSaveOptions och ställ in vattenstämpeln
            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Spara arbetsboken med vattenstämpel
            workbook.Save("WatermarkDemo.pdf", saveOptions);
        }
    }
}
```

### Se även

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## RenderingWatermark(byte[]) {#constructor}

Skapar en instans av bildvattenstämpel.

```csharp
public RenderingWatermark(byte[] imageData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageData | Byte[] |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class RenderingWatermarkMethodCtorWithByteArrayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Förbered bilddata för vattenstämpel
            string imagePath = "watermark.png";
            
            if (!File.Exists(imagePath))
            {
                Console.WriteLine($"Image file not found: {imagePath}");
                return;
            }

            try
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                
                // Skapa RenderingWatermark med Byte[]-konstruktor
                RenderingWatermark watermark = new RenderingWatermark(imageData);
                
                // Konfigurera vattenstämpelns egenskaper
                watermark.Rotation = 45;
                watermark.Opacity = 0.5f;
                watermark.ScaleToPagePercent = 50;
                watermark.IsBackground = true;
                watermark.HAlignment = TextAlignmentType.Center;
                watermark.VAlignment = TextAlignmentType.Center;

                // Skapa PDF-sparalternativ och tillämpa vattenstämpel
                PdfSaveOptions saveOptions = new PdfSaveOptions();
                saveOptions.Watermark = watermark; // Fixed property name

                // Spara arbetsboken med vattenstämpelseffekt
                workbook.Save("WatermarkOutput.pdf", saveOptions);
                
                Console.WriteLine("Watermark applied successfully using Byte[] constructor. Output saved to WatermarkOutput.pdf");
            }
            catch (FileNotFoundException ex)
            {
                Console.WriteLine($"Error loading image file: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RenderingWatermark constructor: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


