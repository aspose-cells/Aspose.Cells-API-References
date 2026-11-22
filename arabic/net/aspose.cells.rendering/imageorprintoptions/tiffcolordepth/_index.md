---
title: "ImageOrPrintOptions.TiffColorDepth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. يحصل أو يضبط عمق البت الذي يُطبق فقط عند حفظ الصفحات بصيغة Tiff"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/tiffcolordepth/
---
## ImageOrPrintOptions.TiffColorDepth property

يحصل أو يضبط عمق البت لتطبيقه فقط عند حفظ الصفحات بصيغة `Tiff`.

```csharp
public ColorDepth TiffColorDepth { get; set; }
```

### ملاحظات

يكون له تأثير فقط عند الحفظ إلى TIFF. إذا تم تعيين TiffCompression إلى CCITT3 أو CCITT4، لن يحدث ذلك، وسيكون عمق البت للصورة tiff المُولدة دائمًا 1.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyTiffColorDepthDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف محتوى مُنسق لعرض عمق اللون
            worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("24-bit Color Depth");
            Style style = cell.GetStyle();
            style.Font.Color = System.Drawing.Color.FromArgb(255, 0, 128, 0);
            style.BackgroundColor = System.Drawing.Color.FromArgb(255, 255, 192, 128);
            style.Pattern = BackgroundType.Solid;
            cell.SetStyle(style);

            // تهيئة ImageOrPrintOptions لتحويل TIFF
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionLZW
            };

            // اعرض وعدل TiffColorDepth
            Console.WriteLine($"Initial TiffColorDepth: {options.TiffColorDepth}");
            
            // حوّل باستخدام العمق الافتراضي (1bpp)
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToTiff("DefaultDepthOutput.tiff");

            // غيّر إلى عمق لون 24‑بت
            options.TiffColorDepth = ColorDepth.Format24bpp;
            Console.WriteLine($"Modified TiffColorDepth: {options.TiffColorDepth}");

            // حوّل بالعمق الجديد
            renderer.ToTiff("24BitDepthOutput.tiff");

            Console.WriteLine("Generated TIFF files with different color depths.");
        }
    }
}
```

### انظر أيضًا

* enum [ColorDepth](../../colordepth/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


