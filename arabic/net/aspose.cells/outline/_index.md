---
title: "فئة Outline"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Outline. تمثل مخططًا في ورقة عمل"
type: docs
url: /ar/net/aspose.cells/outline/
---
## Outline class

يمثل مخططًا على ورقة العمل.

```csharp
public class Outline
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [SummaryColumnRight](../../aspose.cells/outline/summarycolumnright/) { get; set; } | يشير إلى ما إذا كان سيتم وضع عمود الملخص إلى يمين أعمدة التفاصيل في المخطط. |
| [SummaryRowBelow](../../aspose.cells/outline/summaryrowbelow/) { get; set; } | يشير إلى ما إذا كان سيتم وضع صف الملخص أسفل صفوف التفاصيل في المخطط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OutlineDemo
    {
        public static void OutlineExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى في المصنف
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى مخطط ورقة العمل
            Outline outline = worksheet.Outline;
            
            // تعيين خصائص المخطط
            outline.SummaryRowBelow = true; // Indicates if the summary row will be positioned below the detail rows
            outline.SummaryColumnRight = true; // Indicates if the summary column will be positioned to the right of the detail columns
            
            // احفظ المصنف
            workbook.Save("OutlineExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


