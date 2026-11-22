---
title: "Top10Filter.Criteria"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Top10Filter. القيمة الفعلية للخلية في النطاق التي تُستخدم لإجراء المقارنة لهذا الفلتر. هذه هي القيمة المخزنة مؤقتًا أثناء عملية التحديث"
type: docs
url: /ar/net/aspose.cells/top10filter/criteria/
---
## Top10Filter.Criteria property

القيمة الفعلية للخلية في النطاق التي تُستخدم لإجراء المقارنة لهذا الفلتر. هذه هي القيمة المخزنة مؤقتًا أثناء عملية التحديث.

```csharp
[Obsolete("Ignore this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Criteria { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى تجاهل هذه الخاصية. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2025. تقدم Aspose باعتذار عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class Top10FilterPropertyCriteriaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[i, 0].PutValue(20 - i);
            }
            
            worksheet.AutoFilter.Range = "A1:A20";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // تصحيح: الوصول إلى خاصية Filter وتحويلها إلى Top10Filter
            Top10Filter filter = (Top10Filter)worksheet.AutoFilter.FilterColumns[0].Filter;
            Console.WriteLine("Current Criteria value: " + filter.Criteria);
            
            filter.Criteria = 14;
            
            worksheet.AutoFilter.Refresh();
            
            workbook.Save("Top10FilterCriteriaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


