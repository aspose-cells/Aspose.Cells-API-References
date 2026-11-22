---
title: "ImageOrPrintOptions.EmbededImageNameInSvg"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. حدد اسم ملف الصورة المضمنة في svg. يجب أن يكون مسارًا كاملاً مع الدليل مثل cxpsEmbedded"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/
---
## ImageOrPrintOptions.EmbededImageNameInSvg property

حدد اسم ملف الصورة المضمنة في svg. يجب أن يكون مسارًا كاملاً مع الدليل مثل "c:\\xpsEmbedded"

```csharp
[Obsolete("Images are now always embedded in Svg with base64 format, please remove this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EmbededImageNameInSvg { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى إزالة هذه الخاصية لأن الصور الآن دائمًا مضمَّنة في Svg بصيغة base64. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أبريل 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyEmbededImageNameInSvgDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أنشئ صورة بسيطة في الذاكرة وأضفها إلى ورقة العمل
            byte[] redPngBytes = Convert.FromBase64String("iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            worksheet.Pictures.Add(0, 0, new MemoryStream(redPngBytes));

            // أنشئ خيارات تحويل الصورة بصيغة SVG
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Svg
            };

            // اعرض مسار الصورة المضمنة الحالي
            Console.WriteLine("Initial EmbededImageNameInSvg: " + options.EmbededImageNameInSvg);

            // قم بتكوين دليل جديد للصور المضمنة
            string imageDir = "svg_embedded_images/";
            options.EmbededImageNameInSvg = imageDir;
            Directory.CreateDirectory(imageDir);

            // حوّل ورقة العمل إلى SVG باستخدام الخيارات المكوَّنة
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "worksheet_output.svg");

            Console.WriteLine("Generated SVG with embedded images in: " + Path.GetFullPath(imageDir));
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


