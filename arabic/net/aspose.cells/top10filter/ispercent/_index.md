---
title: "Top10Filter.IsPercent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Top10Filter. تشير إلى ما إذا كان سيتم الفلترة بنسبة مئوية لقيمة العمود أم لا"
type: docs
url: /ar/net/aspose.cells/top10filter/ispercent/
---
## Top10Filter.IsPercent property

يشير إلى ما إذا كان يجب تصفية حسب قيمة النسبة المئوية للعمود أم لا

```csharp
public bool IsPercent { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyIsPercentDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
                }
            }

            // تطبيق فلتر أعلى 10 (بدون نسبة مئوية)
            worksheet.AutoFilter.Range = "A1:J10";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // احصل على الفلتر وأظهر خاصية IsPercent
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output False

            // تطبيق فلتر أعلى 10 بنسبة مئوية
            worksheet.AutoFilter.FilterTop10(1, true, true, 20);
            filter = worksheet.AutoFilter.FilterColumns[1].Filter as Top10Filter;
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output True
        }
    }
}
```

### انظر أيضًا

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


