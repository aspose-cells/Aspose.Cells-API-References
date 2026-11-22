---
title: "PageSetup.IsAutomaticPaperSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تشير إلى ما إذا كان حجم الورق تلقائيًا"
type: docs
url: /ar/net/aspose.cells/pagesetup/isautomaticpapersize/
---
## PageSetup.IsAutomaticPaperSize property

يشير إلى ما إذا كان حجم الورق تلقائيًا.

```csharp
public bool IsAutomaticPaperSize { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsAutomaticPaperSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى إعداد الصفحة
            PageSetup pageSetup = worksheet.PageSetup;
            
            // احصل على قيمة حجم الورق التلقائي
            Console.WriteLine("Automatic Paper Size: " + pageSetup.IsAutomaticPaperSize);
            
            // إنشاء مصنف آخر بإعدادات مختلفة
            Workbook workbook2 = new Workbook("example.xlsx");
            PageSetup pageSetup2 = workbook2.Worksheets[0].PageSetup;
            Console.WriteLine("Automatic Paper Size from file: " + pageSetup2.IsAutomaticPaperSize);
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


