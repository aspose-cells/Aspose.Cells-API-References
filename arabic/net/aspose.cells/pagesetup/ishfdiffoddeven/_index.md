---
title: "PageSetup.IsHFDiffOddEven"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. True يعني أن رأس/تذييل الصفحات الفردية مختلف عن الصفحات الزوجية"
type: docs
url: /ar/net/aspose.cells/pagesetup/ishfdiffoddeven/
---
## PageSetup.IsHFDiffOddEven property

صحيح يعني أن الترويسة/التذييل للصفحات الفردية مختلف مع الصفحات الفردية.

```csharp
public bool IsHFDiffOddEven { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffOddEvenDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // تمكين رؤوس/تذييلات مختلفة للصفحات الفردية والزوجية
            pageSetup.IsHFDiffOddEven = true;
            
            // تعيين تذييلات مختلفة للصفحات الفردية والزوجية
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // احفظ المصنف
            workbook.Save("PageSetup_IsHFDiffOddEven_Example.xlsx");
            
            // تحقق من الإعدادات بتحميل الملف المحفوظ
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffOddEven_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            Console.WriteLine("IsHFDiffOddEven: " + loadedPageSetup.IsHFDiffOddEven);
            Console.WriteLine("Odd Page Footer: " + loadedPageSetup.GetFooter(0));
            Console.WriteLine("Even Page Footer: " + loadedPageSetup.GetEvenFooter(0));
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


