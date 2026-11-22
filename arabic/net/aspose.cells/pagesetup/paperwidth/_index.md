---
title: "PageSetup.PaperWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تحصل على عرض الورق بوحدة البوصة مع مراعاة اتجاه الصفحة"
type: docs
url: /ar/net/aspose.cells/pagesetup/paperwidth/
---
## PageSetup.PaperWidth property

يحصل على عرض الورق بوحدة البوصات، مع مراعاة اتجاه الصفحة.

```csharp
public double PaperWidth { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperWidthDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // قم بتعيين بعض البيانات النموذجية
            worksheet.Cells["A1"].PutValue("Sample Page Setup Demo");
            
            // الوصول إلى PageSetup للورقة
            PageSetup pageSetup = worksheet.PageSetup;
            
            // عرض خاصية PaperWidth (للقراءة فقط)
            Console.WriteLine("Paper Width: " + pageSetup.PaperWidth);
            
            // لتغيير حجم الورق، استخدم خاصية PaperSize بدلاً من ذلك
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            Console.WriteLine("New Paper Width: " + pageSetup.PaperWidth);
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


