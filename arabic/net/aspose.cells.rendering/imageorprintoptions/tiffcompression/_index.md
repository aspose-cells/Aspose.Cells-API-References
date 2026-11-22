---
title: "ImageOrPrintOptions.TiffCompression"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تحصل أو تضبط نوع الضغط الذي يُطبق فقط عند حفظ الصفحات بتنسيق Tiff"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/tiffcompression/
---
## ImageOrPrintOptions.TiffCompression property

يحصل أو يضبط نوع الضغط لتطبيقه فقط عند حفظ الصفحات بصيغة `Tiff`.

```csharp
public TiffCompression TiffCompression { get; set; }
```

### ملاحظات

يؤثر فقط عند الحفظ إلى TIFF. القيمة الافتراضية هي Lzw.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTiffCompressionDemo
    {
        public static void Run()
        {
            // إنشاء مصنف تجريبي
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("TIFF Compression Test");

            // تعيين خيارات الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;

            // اختبار أنواع ضغط مختلفة
            string outputPath = "OutputTIFF_";

            options.TiffCompression = TiffCompression.CompressionNone;
            SaveAsTiff(workbook, options, outputPath + "None.tiff");

            options.TiffCompression = TiffCompression.CompressionRle;
            SaveAsTiff(workbook, options, outputPath + "Rle.tiff");

            options.TiffCompression = TiffCompression.CompressionLZW;
            SaveAsTiff(workbook, options, outputPath + "LZW.tiff");

            options.TiffCompression = TiffCompression.CompressionCCITT3;
            SaveAsTiff(workbook, options, outputPath + "CCITT3.tiff");

            options.TiffCompression = TiffCompression.CompressionCCITT4;
            SaveAsTiff(workbook, options, outputPath + "CCITT4.tiff");
        }

        private static void SaveAsTiff(Workbook workbook, ImageOrPrintOptions options, string fileName)
        {
            WorkbookRender renderer = new WorkbookRender(workbook, options);
            renderer.ToImage(fileName);
        }
    }
}
```

### انظر أيضًا

* enum [TiffCompression](../../tiffcompression/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


