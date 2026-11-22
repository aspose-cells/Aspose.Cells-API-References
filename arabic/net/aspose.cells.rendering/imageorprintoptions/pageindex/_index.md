---
title: "ImageOrPrintOptions.PageIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تحصل أو تعيين الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/pageindex/
---
## ImageOrPrintOptions.PageIndex property

يحصل أو يضبط الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها.

```csharp
public int PageIndex { get; set; }
```

### ملاحظات

القيمة الافتراضية هي 0.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية إلى صفحات متعددة
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
            }

            // إعداد خيارات الصورة/الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PageIndex = 1; // Start from second page (0-based index would be 1)
            options.PageCount = 1; // Only process one page

            // إنشاء عرض ورقة للورقة الأولى.
            SheetRender render = new SheetRender(worksheet, options);

            // حفظ إلى PDF باستخدام طريقة API الصحيحة
            render.ToImage(0, "output.pdf");
            Console.WriteLine("Saved page 2 to PDF successfully.");
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


