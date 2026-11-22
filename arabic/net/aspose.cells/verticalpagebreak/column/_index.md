---
title: "VerticalPageBreak.Column"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VerticalPageBreak. يحصل على فهرس العمود لفاصل الصفحة العمودي"
type: docs
url: /ar/net/aspose.cells/verticalpagebreak/column/
---
## VerticalPageBreak.Column property

يحصل على فهرس العمود لفاصل الصفحة العمودي.

```csharp
public int Column { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة فواصل صفحات عمودية في الأعمدة 4 و 8
            worksheet.VerticalPageBreaks.Add(4);
            worksheet.VerticalPageBreaks.Add(8);

            // احصل على مجموعة فواصل الصفحات العمودية
            VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;

            // عرض معلومات حول كل فاصل صفحة عمودي
            Console.WriteLine("Vertical Page Breaks Count: " + vpagebreaks.Count);
            
            foreach (VerticalPageBreak vpagebreak in vpagebreaks)
            {
                Console.WriteLine("\nPage Break at Column: " + vpagebreak.Column);
                Console.WriteLine("Start Row: " + vpagebreak.StartRow);
                Console.WriteLine("End Row: " + vpagebreak.EndRow);
            }

            // احفظ المصنف
            workbook.Save("VerticalPageBreakDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


