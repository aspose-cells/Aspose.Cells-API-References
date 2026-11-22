---
title: "الفئة HorizontalPageBreak"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.HorizontalPageBreak. تغلف الكائن الذي يمثل فاصل صفحة أفقي"
type: docs
url: /ar/net/aspose.cells/horizontalpagebreak/
---
## HorizontalPageBreak class

يغلف الكائن الذي يمثل فاصل صفحة أفقي.

```csharp
public class HorizontalPageBreak
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [EndColumn](../../aspose.cells/horizontalpagebreak/endcolumn/) { get; } | يحصل على فهرس العمود النهائي لهذا الفاصل الأفقي. |
| [Row](../../aspose.cells/horizontalpagebreak/row/) { get; } | يحصل على فهرس الصف المستند إلى الصفر. |
| [StartColumn](../../aspose.cells/horizontalpagebreak/startcolumn/) { get; } | يحصل على فهرس العمود الابتدائي لهذا الفاصل الأفقي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HorizontalPageBreakDemo
    {
        public static void HorizontalPageBreakExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            
            // الحصول على مرجع ورقة العمل التي تم إضافتها حديثًا بتمرير sheet index
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة فاصل صفحة في الخلية Y30
            int index = worksheet.HorizontalPageBreaks.Add("Y30");
            
            // الحصول على الفاصل الأفقي الذي تم إضافته حديثًا
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];
            
            // عرض خصائص الفاصل الأفقي
            Console.WriteLine("Horizontal Page Break Details:");
            Console.WriteLine($"Row: {hPageBreak.Row}");
            Console.WriteLine($"Start Column: {hPageBreak.StartColumn}");
            Console.WriteLine($"End Column: {hPageBreak.EndColumn}");
            
            // احفظ المصنف
            workbook.Save("HorizontalPageBreakExample.xlsx");
            workbook.Save("HorizontalPageBreakExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


