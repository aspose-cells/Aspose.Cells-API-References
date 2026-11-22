---
title: "PageSetup.SetFitToPages"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تحدد عدد الصفحات التي سيتم تحجيم ورقة العمل إليها عند طباعتها"
type: docs
url: /ar/net/aspose.cells/pagesetup/setfittopages/
---
## PageSetup.SetFitToPages method

يضبط عدد الصفحات التي سيتم تحجيم ورقة العمل إليها عند طباعتها.

```csharp
public void SetFitToPages(int wide, int tall)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عريض | Int32 | صفحات عريضة. |
| طويل | Int32 | طويل بالصفحات. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFitToPagesWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى PageSetup للورقة الأولى
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // ضبط إعدادات الملاءمة للصفحات
            setup.SetFitToPages(2, 3);
            
            // تحقق وأخرج الإعدادات
            Console.WriteLine("IsPercentScale: " + setup.IsPercentScale);
            Console.WriteLine("FitToPagesWide: " + setup.FitToPagesWide);
            Console.WriteLine("FitToPagesTall: " + setup.FitToPagesTall);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


