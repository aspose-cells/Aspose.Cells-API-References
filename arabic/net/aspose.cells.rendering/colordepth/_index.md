---
title: "تعداد ColorDepth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Rendering.ColorDepth. يعدد نوع عمق البت لصورة tiff"
type: docs
url: /ar/net/aspose.cells.rendering/colordepth/
---
## ColorDepth enumeration

يعدد نوع عمق البت لصورة TIFF.

```csharp
public enum ColorDepth
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Default | `0` | القيمة الافتراضية، قيمة غير مُحددة. |
| Format1bpp | `1` | 1 بت لكل بكسل |
| Format4bpp | `4` | 4 بتات لكل بكسل |
| Format8bpp | `8` | 8 بتات لكل بكسل |
| Format24bpp | `24` | 24 بت لكل بكسل |
| Format32bpp | `32` | 32 بت لكل بكسل |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;

    public class RenderingClassColorDepthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
            worksheet.Cells["B2"].PutValue(12345);
            
            // تكوين خيارات صورة TIFF
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffColorDepth = ColorDepth.Format8bpp;

            // عرض الورقة إلى TIFF باستخدام عمق اللون المحدد
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_8bpp.tiff");

            // عرض متغيّر آخر لعمق اللون
            options.TiffColorDepth = ColorDepth.Format24bpp;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_24bpp.tiff");

            Console.WriteLine("TIFF files created with different color depths.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


