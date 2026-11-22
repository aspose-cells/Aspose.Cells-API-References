---
title: "PageSetup.PrintQuality"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل جودة الطباعة"
type: docs
url: /ar/net/aspose.cells/pagesetup/printquality/
---
## PageSetup.PrintQuality property

يمثل جودة الطباعة.

```csharp
public int PrintQuality { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintQualityDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ضبط جودة الطباعة إلى 144 نقطة في البوصة
            worksheet.PageSetup.PrintQuality = 144;
            
            // طباعة إعداد جودة الطباعة الحالي
            Console.WriteLine("Print Quality: " + worksheet.PageSetup.PrintQuality);
            
            // احفظ المصنف
            workbook.Save("PrintQualityDemo.xls");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


