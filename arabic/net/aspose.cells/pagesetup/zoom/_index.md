---
title: "PageSetup.Zoom"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل عامل التحجيم بالنسبة المئوية. يجب أن تكون بين 10 و 400"
type: docs
url: /ar/net/aspose.cells/pagesetup/zoom/
---
## PageSetup.Zoom property

يمثل عامل التحجيم بالنسبة المئوية. يجب أن يكون بين 10 و 400.

```csharp
public int Zoom { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyZoomDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ضبط مستوى التكبير إلى 150٪
            worksheet.PageSetup.Zoom = 150;
            
            // طباعة مستوى التكبير الحالي
            Console.WriteLine("Current Zoom Level: " + worksheet.PageSetup.Zoom);
            
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


