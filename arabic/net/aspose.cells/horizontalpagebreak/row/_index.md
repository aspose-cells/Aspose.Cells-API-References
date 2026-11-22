---
title: "HorizontalPageBreak.Row"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HorizontalPageBreak. تُرجع فهرس الصف بدءًا من الصفر"
type: docs
url: /ar/net/aspose.cells/horizontalpagebreak/row/
---
## HorizontalPageBreak.Row property

يحصل على فهرس الصف المستند إلى الصفر.

```csharp
public int Row { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف فواصل صفحات أفقية
            worksheet.HorizontalPageBreaks.Add(6);
            worksheet.HorizontalPageBreaks.Add(12);

            // احصل على مجموعة فواصل الصفحات الأفقية
            HorizontalPageBreakCollection breaks = worksheet.HorizontalPageBreaks;

            // اعرض أرقام الصفوف لفواصل الصفحات
            Console.WriteLine("Page break at row: " + breaks[0].Row);
            Console.WriteLine("Page break at row: " + breaks[1].Row);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


