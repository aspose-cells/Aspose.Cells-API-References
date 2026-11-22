---
title: "VerticalPageBreak.StartRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VerticalPageBreak. يحصل على فهرس الصف الابتدائي لفاصل الصفحة العمودي"
type: docs
url: /ar/net/aspose.cells/verticalpagebreak/startrow/
---
## VerticalPageBreak.StartRow property

يحصل على فهرس الصف الابتدائي لفاصل الصفحة العمودي.

```csharp
public int StartRow { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyStartRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة فواصل صفحات عمودية مع الصف الابتدائي المطلوب (2) في البداية
            worksheet.VerticalPageBreaks.Add(2, 0, 10);
            VerticalPageBreak vPageBreak = worksheet.VerticalPageBreaks[0];

            // عرض خاصية StartRow
            Console.WriteLine("Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // نظرًا لأن StartRow للقراءة فقط، نحتاج إلى إزالته وإعادة إضافته لتغييره
            worksheet.VerticalPageBreaks.RemoveAt(0);
            worksheet.VerticalPageBreaks.Add(5, 0, 10);
            vPageBreak = worksheet.VerticalPageBreaks[0];
            Console.WriteLine("Modified Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // احفظ المصنف
            workbook.Save("VerticalPageBreakExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


