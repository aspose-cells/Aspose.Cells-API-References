---
title: "PageSetup.PaperHeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تحصل على ارتفاع الورق بوحدة البوصة مع اعتبار اتجاه الصفحة"
type: docs
url: /ar/net/aspose.cells/pagesetup/paperheight/
---
## PageSetup.PaperHeight property

يحصل على ارتفاع الورق بوحدة البوصات، مع مراعاة اتجاه الصفحة.

```csharp
public double PaperHeight { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperHeightDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين بعض البيانات في خلية
            worksheet.Cells["A1"].PutValue("Paper Height Demo");
            
            // احصل على كائن PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // عرض ارتفاع الورق الافتراضي (بالبوصة)
            Console.WriteLine("Default Paper Height: " + pageSetup.PaperHeight);
            
            // PaperHeight للقراءة فقط، لذا نوضح الحصول على أحجام ورق مختلفة
            // عن طريق تغيير نوع حجم الورق إلى Letter (8.5×11 بوصة)
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // تحقق من التغيير
            Console.WriteLine("Modified Paper Height (Letter size): " + pageSetup.PaperHeight);
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


