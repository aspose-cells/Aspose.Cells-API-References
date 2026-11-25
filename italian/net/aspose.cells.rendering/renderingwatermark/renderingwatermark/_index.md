---
title: "RenderingWatermark.RenderingWatermark"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore RenderingWatermark. Crea un'istanza della filigrana di testo"
type: docs
url: /it/net/aspose.cells.rendering/renderingwatermark/renderingwatermark/
---
## RenderingWatermark(string, RenderingFont) {#constructor_1}

Crea un'istanza di filigrana testo.

```csharp
public RenderingWatermark(string text, RenderingFont renderingFont)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | String | testo della filigrana |
| renderingFont | RenderingFont | carattere della filigrana |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea un oggetto RenderingFont
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Color = Color.Blue
            };

            // Crea un oggetto RenderingWatermark usando il costruttore #ctor(string, RenderingFont)
            RenderingWatermark watermark = new RenderingWatermark("DEMO WATERMARK", renderingFont)
            {
                Rotation = 45,
                Opacity = 0.3f
            };

            // Crea PdfSaveOptions e imposta la filigrana
            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Salva la cartella di lavoro con filigrana
            workbook.Save("WatermarkDemo.pdf", saveOptions);
        }
    }
}
```

### Vedi anche

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## RenderingWatermark(byte[]) {#constructor}

Crea un'istanza di filigrana immagine.

```csharp
public RenderingWatermark(byte[] imageData)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageData | Byte[] |  |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Prepara i dati immagine per la filigrana
            string imagePath = "watermark.png";
            
            if (!File.Exists(imagePath))
            {
                Console.WriteLine($"Image file not found: {imagePath}");
                return;
            }

            try
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                
                // Crea RenderingWatermark con il costruttore Byte[]
                RenderingWatermark watermark = new RenderingWatermark(imageData);
                
                // Configura le proprietà della filigrana
                watermark.Rotation = 45;
                watermark.Opacity = 0.5f;
                watermark.ScaleToPagePercent = 50;
                watermark.IsBackground = true;
                watermark.HAlignment = TextAlignmentType.Center;
                watermark.VAlignment = TextAlignmentType.Center;

                // Crea le opzioni di salvataggio PDF e applica la filigrana
                PdfSaveOptions saveOptions = new PdfSaveOptions();
                saveOptions.Watermark = watermark; // Fixed property name

                // Salva la cartella di lavoro con effetto filigrana
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

### Vedi anche

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


