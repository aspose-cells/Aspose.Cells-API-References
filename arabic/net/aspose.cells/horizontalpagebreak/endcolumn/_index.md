---
title: "HorizontalPageBreak.EndColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HorizontalPageBreak. تُرجع فهرس العمود النهائي لهذا الفاصل الأفقي"
type: docs
url: /ar/net/aspose.cells/horizontalpagebreak/endcolumn/
---
## HorizontalPageBreak.EndColumn property

يحصل على فهرس العمود النهائي لهذا الفاصل الأفقي.

```csharp
public int EndColumn { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyEndColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف فاصل صفحة أفقي في الصف 5، يمتد من العمود 2 إلى 4
            int index = worksheet.HorizontalPageBreaks.Add(5, 2, 4);
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];

            // اعرض خاصية EndColumn
            Console.WriteLine("Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);

            // نظرًا لأن EndColumn للقراءة فقط، نحتاج إلى إزالة فاصل الصفحة وإعادة إضافته لتعديله
            worksheet.HorizontalPageBreaks.RemoveAt(index);
            index = worksheet.HorizontalPageBreaks.Add(5, 2, 6);
            hPageBreak = worksheet.HorizontalPageBreaks[index];
            Console.WriteLine("Modified Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);
        }
    }
}
```

### انظر أيضًا

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


