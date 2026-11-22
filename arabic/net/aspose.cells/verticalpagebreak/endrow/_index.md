---
title: "VerticalPageBreak.EndRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VerticalPageBreak. يحصل على فهرس الصف النهائي لفاصل الصفحة العمودي"
type: docs
url: /ar/net/aspose.cells/verticalpagebreak/endrow/
---
## VerticalPageBreak.EndRow property

يحصل على فهرس الصف النهائي لفاصل الصفحة العمودي.

```csharp
public int EndRow { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyEndRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة فاصل صفحة عمودي يمتد من الصفوف 3 إلى 8 في العمود C (الفهرس 2)
            worksheet.VerticalPageBreaks.Add("C3:C8");

            // احصل على أول فاصل صفحة عمودي
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
            
            // عرض الصف النهائي لفاصل الصفحة
            Console.WriteLine("Vertical Page Break End Row: " + vpb.EndRow);
            
            // نظرًا لأن EndRow للقراءة فقط، سنوضح كيفية الحصول عليه دون تعيينه
            // السطر التالي تم إزالته لأنه يسبب خطأ في التجميع:
            // vpb.EndRow = 10;
            
            // بدلاً من ذلك، سنضيف فاصل صفحة آخر بصف نهائي مختلف
            worksheet.VerticalPageBreaks.Add("C3:C10");
            VerticalPageBreak vpb2 = worksheet.VerticalPageBreaks[1];
            Console.WriteLine("Second Page Break End Row: " + vpb2.EndRow);
        }
    }
}
```

### انظر أيضًا

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


