---
title: "PageSetup.IsHFDiffFirst"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. True تعني أن رأس/تذييل الصفحة الأولى مختلف عن الصفحات الأخرى"
type: docs
url: /ar/net/aspose.cells/pagesetup/ishfdifffirst/
---
## PageSetup.IsHFDiffFirst property

صحيح يعني أن الترويسة/التذييل للصفحة الأولى مختلف عن الصفحات الأخرى.

```csharp
public bool IsHFDiffFirst { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffFirstDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // تعيين رؤوس/تذييلات مختلفة للصفحة الأولى
            pageSetup.IsHFDiffFirst = true;
            
            // عيّن الرؤوس/التذييلات
            pageSetup.SetFirstPageHeader(0, "First Page Header");
            pageSetup.SetHeader(0, "Standard Header");
            
            // احفظ المصنف
            workbook.Save("PageSetup_IsHFDiffFirst_Example.xlsx");
            
            // إعادة تحميل الدفتر للتحقق من الإعدادات
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffFirst_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            // أخرج التحقق
            Console.WriteLine("IsHFDiffFirst: " + loadedPageSetup.IsHFDiffFirst);
            Console.WriteLine("First Page Header: " + loadedPageSetup.GetFirstPageHeader(0));
            Console.WriteLine("Standard Header: " + loadedPageSetup.GetHeader(0));
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


