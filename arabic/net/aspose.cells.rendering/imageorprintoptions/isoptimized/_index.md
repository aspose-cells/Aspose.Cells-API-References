---
title: "ImageOrPrintOptions.IsOptimized"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تشير إلى ما إذا كان يجب تحسين العناصر الناتجة"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/isoptimized/
---
## ImageOrPrintOptions.IsOptimized property

يحدد ما إذا كان سيتم تحسين عناصر الإخراج.

```csharp
public bool IsOptimized { get; set; }
```

### ملاحظات

القيمة الافتراضية هي false. حاليًا عندما يتم تعيين هذه الخاصية إلى true، سيتم تنفيذ التحسينات التالية: 1. تحسين خطوط الحدود. 2. تحسين حجم الملف أثناء العرض إلى صورة Svg.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyIsOptimizedDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i}-{j}");
                }
            }

            // إعداد خيارات عرض الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // توضيح خاصية IsOptimized
            options.IsOptimized = true; // Enable optimization
            
            // تحويل الورقة إلى صورة
            SheetRender renderer = new SheetRender(sheet, options);
            MemoryStream stream = new MemoryStream();
            renderer.ToImage(0, stream);
            
            Console.WriteLine($"Image rendered with optimization: {options.IsOptimized}");
            Console.WriteLine($"Image size: {stream.Length} bytes");
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


