---
title: "RenderingWatermark.RenderingWatermark"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RenderingWatermark yapıcı. Metin filigranının bir örneğini oluşturur"
type: docs
url: /tr/net/aspose.cells.rendering/renderingwatermark/renderingwatermark/
---
## RenderingWatermark(string, RenderingFont) {#constructor_1}

Metin filigranı örneği oluşturur.

```csharp
public RenderingWatermark(string text, RenderingFont renderingFont)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | String | filigran metni |
| renderingFont | RenderingFont | filigran yazı tipi |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Bir RenderingFont nesnesi oluştur
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Color = Color.Blue
            };

            // Bir RenderingWatermark nesnesi oluşturmak için #ctor(string, RenderingFont) kullan
            RenderingWatermark watermark = new RenderingWatermark("DEMO WATERMARK", renderingFont)
            {
                Rotation = 45,
                Opacity = 0.3f
            };

            // PdfSaveOptions oluştur ve filigranı ayarla
            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Çalışma kitabını filigran ile kaydet
            workbook.Save("WatermarkDemo.pdf", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## RenderingWatermark(byte[]) {#constructor}

Görüntü filigranı örneği oluşturur.

```csharp
public RenderingWatermark(byte[] imageData)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| imageData | Byte[] |  |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Filigran için görüntü verisini hazırla
            string imagePath = "watermark.png";
            
            if (!File.Exists(imagePath))
            {
                Console.WriteLine($"Image file not found: {imagePath}");
                return;
            }

            try
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                
                // Byte[] yapıcı ile RenderingWatermark oluştur
                RenderingWatermark watermark = new RenderingWatermark(imageData);
                
                // Filigran özelliklerini yapılandır
                watermark.Rotation = 45;
                watermark.Opacity = 0.5f;
                watermark.ScaleToPagePercent = 50;
                watermark.IsBackground = true;
                watermark.HAlignment = TextAlignmentType.Center;
                watermark.VAlignment = TextAlignmentType.Center;

                // PDF kaydetme seçeneklerini oluştur ve filigranı uygula
                PdfSaveOptions saveOptions = new PdfSaveOptions();
                saveOptions.Watermark = watermark; // Fixed property name

                // Çalışma kitabını filigran etkisiyle kaydet
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

### Ayrıca Bakınız

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


