---
title: "RenderingWatermark.Image"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RenderingWatermark. تحصل على صورة العلامة المائية"
type: docs
url: /ar/net/aspose.cells.rendering/renderingwatermark/image/
---
## RenderingWatermark.Image property

يحصل على صورة العلامة المائية.

```csharp
public byte[] Image { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System.IO;

    public class RenderingWatermarkPropertyImageDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحميل بيانات الصورة من الملف
            byte[] originalImage = File.ReadAllBytes("watermark.png");

            // إنشاء علامة مائية مستندة إلى الصورة مع الصورة الأولية
            RenderingWatermark watermark = new RenderingWatermark(originalImage);
            Console.WriteLine("Initial image size: " + watermark.Image.Length + " bytes");

            // تعديل خصائص العلامة المائية
            watermark.Rotation = 45f;
            watermark.Opacity = 0.5f;
            watermark.ScaleToPagePercent = 75;
            watermark.IsBackground = true;
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;

            // إنشاء خيارات حفظ PDF مع العلامة المائية
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Watermark = watermark; // Fixed property name

            // حفظ إلى PDF مع إخراج مائي
            workbook.Save("WatermarkedOutput.pdf", pdfOptions);

            // إنشاء علامة مائية جديدة بصورة مختلفة
            byte[] updatedImage = File.ReadAllBytes("updated_watermark.png");
            RenderingWatermark newWatermark = new RenderingWatermark(updatedImage);
            Console.WriteLine("Updated image size: " + newWatermark.Image.Length + " bytes");

            // حفظ مع علامة مائية جديدة
            pdfOptions.Watermark = newWatermark; // Fixed property name
            workbook.Save("UpdatedWatermark.pdf", pdfOptions);
        }
    }
}
```

### انظر أيضًا

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


