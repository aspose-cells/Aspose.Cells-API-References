---
title: "PageSetup.GetEvenHeader"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. يحصل على نص ينسق رأس الصفحة الزوجية لملف Excel"
type: docs
url: /ar/net/aspose.cells/pagesetup/getevenheader/
---
## PageSetup.GetEvenHeader method

يحصل على برنامج نصي ينسق الرأس الزوجي لملف Excel.

```csharp
public string GetEvenHeader(int section)
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
    public class PageSetupMethodGetEvenHeaderWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تمكين رؤوس/تذييلات الصفحات الفردية والزوجية المختلفة
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.IsHFDiffOddEven = true;
            
            // ضبط رأس الصفحة الزوجية
            pageSetup.SetEvenHeader(0, "&CEven Page Header Center");
            pageSetup.SetEvenHeader(1, "&LEven Page Header Left");
            pageSetup.SetEvenHeader(2, "&REven Page Header Right");
            
            // احصل على رؤوس الصفحات الزوجية واطبعها
            Console.WriteLine("Even Header Center: " + pageSetup.GetEvenHeader(0));
            Console.WriteLine("Even Header Left: " + pageSetup.GetEvenHeader(1));
            Console.WriteLine("Even Header Right: " + pageSetup.GetEvenHeader(2));
            
            // احفظ المصنف
            workbook.Save("PageSetup_GetEvenHeaderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


