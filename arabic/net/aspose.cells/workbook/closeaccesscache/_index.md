---
title: "Workbook.CloseAccessCache"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تغلق الجلسة التي تستخدم الذاكرات المؤقتة للوصول إلى البيانات"
type: docs
url: /ar/net/aspose.cells/workbook/closeaccesscache/
---
## Workbook.CloseAccessCache method

يغلق الجلسة التي تستخدم الذاكرات المؤقتة للوصول إلى البيانات.

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
    public class WorkbookMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // أضف بيانات عينة وتنسيق شرطي
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i % 2 == 0 ? "Data" : "Other");
            }

            // إضافة تنسيق شرطي
            int ruleIdx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[ruleIdx];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Equal, "Data", null);
            Style style = workbook.CreateStyle();
            style.Font.Size = 16;
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 9, EndColumn = 0 });
            fcc[0].Style = style;

            // بدء ذاكرة الوصول المؤقت للتنسيق الشرطي
            workbook.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // الوصول إلى الخلايا مع تنسيق شرطي مخزن مؤقتًا
            for (int i = 0; i < 10; i++)
            {
                Cell cell = cells[i, 0];
                Console.WriteLine($"Cell {cell.Name}: Value={cell.StringValue}, FontSize={cell.GetDisplayStyle().Font.Size}");
            }

            // إغلاق ذاكرة الوصول المؤقتة
            workbook.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


