---
title: "Worksheet.CloseAccessCache"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تغلق الجلسة التي تستخدم الذاكرات المؤقتة للوصول إلى البيانات في هذه ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/closeaccesscache/
---
## Worksheet.CloseAccessCache method

يغلق الجلسة التي تستخدم الذاكرة المؤقتة للوصول إلى البيانات في هذه ورقة العمل.

```csharp
public void CloseAccessCache(AccessCacheOptions opts)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| opts | AccessCacheOptions | خيارات الوصول إلى البيانات |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // املأ الخلايا ببيانات تجريبية
            for (int i = 0; i < 1000; i++)
            {
                cells[i, 0].PutValue(i % 10);
            }

            // إضافة تنسيق شرطي
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 999, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // تمكين ذاكرة الوصول المؤقتة للتنسيق الشرطي
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // أجرِ عمليات باستخدام الوصول المؤقت
            Random random = new Random();
            for (int i = 0; i < 100; i++)
            {
                int r = random.Next(0, 1000);
                var style = cells[r, 0].GetDisplayStyle();
                Console.WriteLine($"Cell ({r},0) style: {style.ForegroundArgbColor:X}");
            }

            // إغلاق ذاكرة الوصول المؤقتة
            sheet.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);
        }
    }
}
```

### انظر أيضًا

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


