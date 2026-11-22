---
title: "Worksheet.Outline"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. يحصل على المخطط التفصيلي في هذه ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/outline/
---
## Worksheet.Outline property

يحصل على المخطط في ورقة العمل هذه.

```csharp
public Outline Outline { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyOutlineDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية وأنشئ مجموعات المخطط التفصيلي
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[$"A{i + 1}"].Value = $"Item {i + 1}";
                worksheet.Cells[$"B{i + 1}"].Value = (i + 1) * 100;
            }

            // تجميع الصفوف (ينشئ مخططًا تفصيليًا)
            worksheet.Cells.GroupRows(0, 9, false);

            // الوصول إلى خصائص المخطط التفصيلي
            Outline outline = worksheet.Outline;
            Console.WriteLine($"Outline summary row is below detail: {outline.SummaryRowBelow}");
            Console.WriteLine($"Outline summary column is to right: {outline.SummaryColumnRight}");

            // تغيير إعدادات المخطط التفصيلي
            outline.SummaryRowBelow = true;
            outline.SummaryColumnRight = false;

            // إلغاء تجميع الصفوف لتوضيح وظيفة المخطط التفصيلي
            worksheet.Cells.UngroupRows(0, 9);

            // احفظ المصنف
            workbook.Save("WorksheetOutlineDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Outline](../../outline/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


