---
title: "تعداد TiffCompression"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Rendering.TiffCompression. يحدد نوع الضغط الذي يجب تطبيقه عند حفظ الصور في ملف بصيغة TIFF"
type: docs
url: /ar/net/aspose.cells.rendering/tiffcompression/
---
## TiffCompression enumeration

يحدد نوع الضغط الذي يجب تطبيقه عند حفظ الصور في ملف بصيغة TIFF.

```csharp
public enum TiffCompression
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| CompressionNone | `0` | يحدد عدم وجود ضغط. |
| CompressionRle | `1` | يحدد نظام ضغط RLE. |
| CompressionLZW | `2` | يحدد نظام ضغط LZW. |
| CompressionCCITT3 | `3` | يحدد نظام ضغط CCITT3. |
| CompressionCCITT4 | `4` | يحدد نظام ضغط CCITT4. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingClassTiffCompressionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("TIFF Compression Test");
            ws.Cells["A2"].PutValue(DateTime.Now.ToString());

            // تعيين خيارات الصورة
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;
            imgOpt.ImageType = ImageType.Tiff;

            // اختبار أنواع ضغط مختلفة
            string outputPath = "output_compression_";

            // ضغط LZW
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "LZW.tiff");

            // ضغط CCITT3
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT3;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT3.tiff");

            // ضغط CCITT4
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT4;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT4.tiff");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


