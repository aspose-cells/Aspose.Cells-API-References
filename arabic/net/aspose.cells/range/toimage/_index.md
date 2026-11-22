---
title: "Range.ToImage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. يحول النطاق إلى صورة"
type: docs
url: /ar/net/aspose.cells/range/toimage/
---
## Range.ToImage method

يقوم بتحويل النطاق إلى صورة.

```csharp
public byte[] ToImage(ImageOrPrintOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيارات | ImageOrPrintOptions | الخيارات لتحويل هذا النطاق إلى صورة |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RangeMethodToImageWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا من ملف Excel نموذجي
            Workbook workbook = new Workbook("example.xlsx");
            
            // احصل على الورقة الأولى وخلاياها
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // أنشئ نطاق A1:J25
            Aspose.Cells.Range range = cells.CreateRange("A1:J25");
            
            // إنشاء خيارات الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions()
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            
            // حوّل النطاق إلى صورة
            byte[] imageData = range.ToImage(options);
            
            // احفظ الصورة إلى ملف
            File.WriteAllBytes("range_output.png", imageData);
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


