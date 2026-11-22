---
title: "الفئة VerticalPageBreak"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.VerticalPageBreak. تغلف الكائن الذي يمثل فاصل صفحة عمودي"
type: docs
url: /ar/net/aspose.cells/verticalpagebreak/
---
## VerticalPageBreak class

يحتوي على الكائن الذي يمثل فاصل صفحة عمودي.

```csharp
public class VerticalPageBreak
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Column](../../aspose.cells/verticalpagebreak/column/) { get; } | يحصل على فهرس العمود لفاصل الصفحة العمودي. |
| [EndRow](../../aspose.cells/verticalpagebreak/endrow/) { get; } | يحصل على فهرس الصف النهائي لفاصل الصفحة العمودي. |
| [StartRow](../../aspose.cells/verticalpagebreak/startrow/) { get; } | يحصل على فهرس الصف الابتدائي لفاصل الصفحة العمودي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakDemo
    {
        public static void VerticalPageBreakExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى في المصنف
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة فاصل صفحة عمودي عند العمود G (الفهرس 6)
            worksheet.VerticalPageBreaks.Add("G5");

            // احفظ المصنف
            workbook.Save("VerticalPageBreakExample.xlsx");

            // الوصول إلى فاصل الصفحة العمودي المضاف
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];

            // عرض خصائص فاصل الصفحة العمودي
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


