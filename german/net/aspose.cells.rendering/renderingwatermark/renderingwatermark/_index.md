---
title: "RenderingWatermark.RenderingWatermark"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingWatermark-Konstruktor. Erstellt eine Instanz eines Textwasserzeichens"
type: docs
url: /de/net/aspose.cells.rendering/renderingwatermark/renderingwatermark/
---
## RenderingWatermark(string, RenderingFont) {#constructor_1}

Erstellt eine Instanz eines Textwasserzeichens.

```csharp
public RenderingWatermark(string text, RenderingFont renderingFont)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | String | Wasserzeichentext |
| renderingFont | RenderingFont | Wasserzeichen-Schriftart |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Erstelle ein RenderingFont-Objekt
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Color = Color.Blue
            };

            // Erstelle ein RenderingWatermark-Objekt mit dem #ctor(string, RenderingFont)
            RenderingWatermark watermark = new RenderingWatermark("DEMO WATERMARK", renderingFont)
            {
                Rotation = 45,
                Opacity = 0.3f
            };

            // Erstelle PdfSaveOptions und setze das Wasserzeichen
            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Speichere die Arbeitsmappe mit Wasserzeichen
            workbook.Save("WatermarkDemo.pdf", saveOptions);
        }
    }
}
```

### Siehe auch

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## RenderingWatermark(byte[]) {#constructor}

Erstellt eine Instanz eines Bildwasserzeichens.

```csharp
public RenderingWatermark(byte[] imageData)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageData | Byte[] |  |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bereite Bilddaten für das Wasserzeichen vor
            string imagePath = "watermark.png";
            
            if (!File.Exists(imagePath))
            {
                Console.WriteLine($"Image file not found: {imagePath}");
                return;
            }

            try
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                
                // Erstelle RenderingWatermark mit dem Byte[]-Konstruktor
                RenderingWatermark watermark = new RenderingWatermark(imageData);
                
                // Konfiguriere die Wasserzeichen-Eigenschaften
                watermark.Rotation = 45;
                watermark.Opacity = 0.5f;
                watermark.ScaleToPagePercent = 50;
                watermark.IsBackground = true;
                watermark.HAlignment = TextAlignmentType.Center;
                watermark.VAlignment = TextAlignmentType.Center;

                // Erstelle PDF-Speicheroptionen und wende das Wasserzeichen an
                PdfSaveOptions saveOptions = new PdfSaveOptions();
                saveOptions.Watermark = watermark; // Fixed property name

                // Speichere die Arbeitsmappe mit Wasserzeichen-Effekt
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

### Siehe auch

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


