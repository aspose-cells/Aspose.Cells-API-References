---
title: "الفئة Top10Filter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Top10Filter. تمثّل أعلى N بالمئة أو عدد العناصر لتصفية حسبها"
type: docs
url: /ar/net/aspose.cells/top10filter/
---
## Top10Filter class

يمثل أعلى N (نسبة مئوية أو عدد العناصر) للتصفية.

```csharp
public class Top10Filter
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Criteria](../../aspose.cells/top10filter/criteria/) { get; set; } | (**Obsolete.**) القيمة الفعلية للخلية في النطاق المستخدمة لإجراء المقارنة لهذا الفلتر. هذه هي قيمة التخزين المؤقت أثناء عملية التحديث. |
| [IsPercent](../../aspose.cells/top10filter/ispercent/) { get; set; } | يشير إلى ما إذا كان يجب تصفية حسب قيمة النسبة المئوية للعمود أم لا |
| [IsTop](../../aspose.cells/top10filter/istop/) { get; set; } | يشير إلى ما إذا كان يجب تصفية حسب الترتيب الأعلى أم لا |
| [Items](../../aspose.cells/top10filter/items/) { get; set; } | يحصل ويعيّن القيمة العليا أو السفلى لاستخدامها كمعيار للفلتر. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTop10FilterDemo
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
                worksheet.Cells["C" + i].PutValue("Item " + (i-6));
            }
            
            // طبق الفلتر التلقائي وفلتر أعلى 10
            worksheet.AutoFilter.Range = "B6:C16";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5); // Filter top 5 values in column B
            
            // احصل على Top10Filter وتحقق من خصائصه
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent);
            Console.WriteLine("Items: " + filter.Items);
            
            // قم بتحديث الفلتر وتحقق من الصفوف المخفية
            worksheet.AutoFilter.Refresh();
            for (int i = 6; i <= 16; i++)
            {
                Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
            }
            
            // احفظ المصنف
            workbook.Save("Top10FilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


