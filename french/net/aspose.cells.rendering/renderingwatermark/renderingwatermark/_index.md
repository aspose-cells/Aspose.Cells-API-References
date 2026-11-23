---
title: "RenderingWatermark.RenderingWatermark"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur RenderingWatermark. Crée une instance du filigrane texte"
type: docs
url: /fr/net/aspose.cells.rendering/renderingwatermark/renderingwatermark/
---
## RenderingWatermark(string, RenderingFont) {#constructor_1}

Crée une instance de filigrane texte.

```csharp
public RenderingWatermark(string text, RenderingFont renderingFont)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| texte | String | texte du filigrane |
| renderingFont | RenderingFont | police du filigrane |

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crée un objet RenderingFont
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Color = Color.Blue
            };

            // Créer un objet RenderingWatermark en utilisant le #ctor(string, RenderingFont)
            RenderingWatermark watermark = new RenderingWatermark("DEMO WATERMARK", renderingFont)
            {
                Rotation = 45,
                Opacity = 0.3f
            };

            // Crée PdfSaveOptions et définit le filigrane
            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Enregistrer le classeur avec filigrane
            workbook.Save("WatermarkDemo.pdf", saveOptions);
        }
    }
}
```

### Voir aussi

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## RenderingWatermark(byte[]) {#constructor}

Crée une instance de filigrane image.

```csharp
public RenderingWatermark(byte[] imageData)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| imageData | Byte[] |  |

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Préparer les données d'image pour le filigrane
            string imagePath = "watermark.png";
            
            if (!File.Exists(imagePath))
            {
                Console.WriteLine($"Image file not found: {imagePath}");
                return;
            }

            try
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                
                // Créer RenderingWatermark avec le constructeur Byte[]
                RenderingWatermark watermark = new RenderingWatermark(imageData);
                
                // Configurer les propriétés du filigrane
                watermark.Rotation = 45;
                watermark.Opacity = 0.5f;
                watermark.ScaleToPagePercent = 50;
                watermark.IsBackground = true;
                watermark.HAlignment = TextAlignmentType.Center;
                watermark.VAlignment = TextAlignmentType.Center;

                // Créer les options d'enregistrement PDF et appliquer le filigrane
                PdfSaveOptions saveOptions = new PdfSaveOptions();
                saveOptions.Watermark = watermark; // Fixed property name

                // Enregistrer le classeur avec l'effet de filigrane
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

### Voir aussi

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


