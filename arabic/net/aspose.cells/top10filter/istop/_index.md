---
title: "Top10Filter.IsTop"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Top10Filter. تشير إلى ما إذا كان سيتم الفلترة حسب الترتيب الأعلى أم لا"
type: docs
url: /ar/net/aspose.cells/top10filter/istop/
---
## Top10Filter.IsTop property

يشير إلى ما إذا كان يجب تصفية حسب الترتيب الأعلى أم لا

```csharp
public bool IsTop { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyIsTopDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["B6"].PutValue("Value");
            for (int i = 7; i <= 16; i++)
            {
                worksheet.Cells["B" + i].PutValue(20 - i);
            }

            // تطبيق فلتر أعلى 5
            worksheet.AutoFilter.Range = "B6:B16";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // احصل على الفلتر وتحقق من خاصية IsTop
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop); // Should output "True"
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output "False"
            
            // تحديث الفلتر والتحقق من الصفوف المخفية
            worksheet.AutoFilter.Refresh();
            for (int i = 6; i <= 16; i++)
            {
                Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


