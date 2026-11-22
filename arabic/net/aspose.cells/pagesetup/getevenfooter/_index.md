---
title: "PageSetup.GetEvenFooter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تحصل على نص ينسق تذييل الصفحات الزوجية لملف Excel"
type: docs
url: /ar/net/aspose.cells/pagesetup/getevenfooter/
---
## PageSetup.GetEvenFooter method

يحصل على برنامج نصي ينسق التذييل الزوجي لملف Excel.

```csharp
public string GetEvenFooter(int section)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| قسم | Int32 | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetEvenFooterWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // تمكين رؤوس/تذييلات مختلفة للصفحات الفردية والزوجية
            pageSetup.IsHFDiffOddEven = true;
            
            // تعيين تذييل الصفحات الزوجية
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // الحصول على وعرض تذييل الصفحات الزوجية
            string evenFooter = pageSetup.GetEvenFooter(0);
            Console.WriteLine("Even Footer: " + evenFooter);
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


