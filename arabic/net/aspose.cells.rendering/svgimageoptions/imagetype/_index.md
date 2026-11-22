---
title: "SvgImageOptions.ImageType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SvgImageOptions. يحصل أو يحدد تنسيق الصور المولدة. القيمة الافتراضية PNG"
type: docs
url: /ar/net/aspose.cells.rendering/svgimageoptions/imagetype/
---
## SvgImageOptions.ImageType property

يحصل أو يضبط تنسيق الصور المُولدة. القيمة الافتراضية: PNG.

```csharp
public override ImageType ImageType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SvgImageOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة وصورة
            worksheet.Cells["A1"].PutValue("Embedded Image Type Demonstration");
            int pictureIndex = worksheet.Pictures.Add(0, 1, "inputImage.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // إنشاء خيارات عرض SVG
            SvgImageOptions svgOptions = new SvgImageOptions();

            // عرض ImageType الحالي (القيمة الافتراضية: PNG)
            Console.WriteLine("Current ImageType: " + svgOptions.ImageType);

            // تغيير تنسيق الصورة للصور النقطية المضمنة
            svgOptions.ImageType = ImageType.Jpeg;

            // حفظ محتوى ورقة العمل كـ SVG بتنسيقات صور مختلفة
            using (MemoryStream stream = new MemoryStream())
            {
                picture.ToImage(stream, svgOptions);
                File.WriteAllBytes("output_with_jpeg.svg", stream.ToArray());
            }

            // إعادة تعيين إلى تنسيق PNG
            svgOptions.ImageType = ImageType.Png;
            
            using (MemoryStream stream = new MemoryStream())
            {
                picture.ToImage(stream, svgOptions);
                File.WriteAllBytes("output_with_png.svg", stream.ToArray());
            }

            Console.WriteLine("SVG files created with different embedded image formats.");
        }
    }
}
```

### انظر أيضًا

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


