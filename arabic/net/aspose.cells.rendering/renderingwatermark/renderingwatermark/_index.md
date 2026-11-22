---
title: "RenderingWatermark.RenderingWatermark"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ RenderingWatermark. ينشئ نسخة من علامة مائية نصية"
type: docs
url: /ar/net/aspose.cells.rendering/renderingwatermark/renderingwatermark/
---
## RenderingWatermark(string, RenderingFont) {#constructor_1}

ينشئ كائنًا من العلامة المائية النصية.

```csharp
public RenderingWatermark(string text, RenderingFont renderingFont)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | String | نص العلامة المائية |
| renderingFont | RenderingFont | خط العلامة المائية |

### أمثلة

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
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء كائن RenderingFont
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Color = Color.Blue
            };

            // إنشاء كائن RenderingWatermark باستخدام #ctor(string, RenderingFont)
            RenderingWatermark watermark = new RenderingWatermark("DEMO WATERMARK", renderingFont)
            {
                Rotation = 45,
                Opacity = 0.3f
            };

            // إنشاء PdfSaveOptions وتعيين العلامة المائية
            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // حفظ المصنف مع العلامة المائية
            workbook.Save("WatermarkDemo.pdf", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## RenderingWatermark(byte[]) {#constructor}

ينشئ كائنًا من العلامة المائية الصورة.

```csharp
public RenderingWatermark(byte[] imageData)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| imageData | Byte[] |  |

### أمثلة

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
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تحضير بيانات الصورة للعلامة المائية
            string imagePath = "watermark.png";
            
            if (!File.Exists(imagePath))
            {
                Console.WriteLine($"Image file not found: {imagePath}");
                return;
            }

            try
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                
                // إنشاء RenderingWatermark باستخدام منشئ Byte[]
                RenderingWatermark watermark = new RenderingWatermark(imageData);
                
                // تكوين خصائص العلامة المائية
                watermark.Rotation = 45;
                watermark.Opacity = 0.5f;
                watermark.ScaleToPagePercent = 50;
                watermark.IsBackground = true;
                watermark.HAlignment = TextAlignmentType.Center;
                watermark.VAlignment = TextAlignmentType.Center;

                // إنشاء خيارات حفظ PDF وتطبيق العلامة المائية
                PdfSaveOptions saveOptions = new PdfSaveOptions();
                saveOptions.Watermark = watermark; // Fixed property name

                // حفظ المصنف مع تأثير العلامة المائية
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

### انظر أيضًا

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


