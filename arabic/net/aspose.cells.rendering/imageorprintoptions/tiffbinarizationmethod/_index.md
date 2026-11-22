---
title: "ImageOrPrintOptions.TiffBinarizationMethod"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. يحصل أو يعيّن الطريقة المستخدمة أثناء تحويل الصور إلى صيغة 1 ببت عندما يكون ImageType هو Tiff و TiffCompression يساوي Ccitt3 أو Ccitt4"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/
---
## ImageOrPrintOptions.TiffBinarizationMethod property

يحصل أو يعيّن الطريقة المستخدمة أثناء تحويل الصور إلى صيغة 1 ببت عندما يكون [`ImageType`](../imagetype/) هو Tiff و [`TiffCompression`](../tiffcompression/) يساوي Ccitt3 أو Ccitt4.

```csharp
public ImageBinarizationMethod TiffBinarizationMethod { get; set; }
```

### ملاحظات

القيمة الافتراضية هي FloydSteinbergDithering.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyTiffBinarizationMethodDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات التدرج للعرض البصري
            for (int i = 0; i < 15; i++)
            {
                Cell cell = worksheet.Cells[i, 0];
                cell.PutValue(i * 7);
                Style style = cell.GetStyle();
                style.BackgroundColor = Color.FromArgb(i * 18, i * 18, i * 18);
                cell.SetStyle(style);
            }

            // تكوين خيارات عرض TIFF
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT3,
                TiffColorDepth = ColorDepth.Format1bpp
            };

            // عرض طريقة الثنائي الحالية
            Console.WriteLine("Initial TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // عرض باستخدام طريقة العتبة الافتراضية
            new SheetRender(worksheet, options).ToImage(0, "ThresholdBinarization.tiff");

            // غيّر إلى Floyd-Steinberg dithering
            options.TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering;
            Console.WriteLine("\nModified TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // عرض باستخدام طريقة جديدة
            new SheetRender(worksheet, options).ToImage(0, "DitheringBinarization.tiff");

            Console.WriteLine("\nGenerated TIFF files demonstrate different 1bpp conversion methods.");
        }
    }
}
```

### انظر أيضًا

* enum [ImageBinarizationMethod](../../imagebinarizationmethod/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


