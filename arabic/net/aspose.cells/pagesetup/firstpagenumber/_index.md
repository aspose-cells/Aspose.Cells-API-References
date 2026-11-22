---
title: "PageSetup.FirstPageNumber"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل رقم الصفحة الأولى الذي سيُستخدم عند طباعة هذه الورقة"
type: docs
url: /ar/net/aspose.cells/pagesetup/firstpagenumber/
---
## PageSetup.FirstPageNumber property

يمثل رقم الصفحة الأولى الذي سيُستخدم عند طباعة هذه الورقة.

```csharp
public int FirstPageNumber { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFirstPageNumberDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين خصائص إعداد الصفحة
            worksheet.PageSetup.IsAutoFirstPageNumber = false;
            worksheet.PageSetup.FirstPageNumber = 3;
            
            // اطبع النتائج
            Console.WriteLine("IsAutoFirstPageNumber: " + worksheet.PageSetup.IsAutoFirstPageNumber);
            Console.WriteLine("FirstPageNumber: " + worksheet.PageSetup.FirstPageNumber);
            
            // احفظ المصنف
            workbook.Save("PageSetupFirstPageNumberDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


