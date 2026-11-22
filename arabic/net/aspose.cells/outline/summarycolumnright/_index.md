---
title: "Outline.SummaryColumnRight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Outline. تشير إلى ما إذا كان عمود الملخص سيُوضع إلى يمين أعمدة التفاصيل في المخطط"
type: docs
url: /ar/net/aspose.cells/outline/summarycolumnright/
---
## Outline.SummaryColumnRight property

يشير إلى ما إذا كان سيتم وضع عمود الملخص إلى يمين أعمدة التفاصيل في المخطط.

```csharp
public bool SummaryColumnRight { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OutlinePropertySummaryColumnRightDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات تجريبية وتجمّيع الصفوف
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + (i + 1));
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // تجميع الصفوف (ينشئ مخططًا)
            worksheet.Cells.GroupRows(0, 9, false);

            // الحصول على إعدادات المخطط
            Outline outline = worksheet.Outline;

            // تعيين SummaryColumnRight إلى true (ستظهر أعمدة الملخص إلى يمين أعمدة التفاصيل)
            outline.SummaryColumnRight = true;
            Console.WriteLine("SummaryColumnRight is set to: " + outline.SummaryColumnRight);

            // احفظ المصنف
            workbook.Save("OutlinePropertySummaryColumnRightDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


