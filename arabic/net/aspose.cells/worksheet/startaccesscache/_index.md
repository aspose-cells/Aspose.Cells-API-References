---
title: "Worksheet.StartAccessCache"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تبدأ الجلسة التي تستخدم الذاكرات المؤقتة للوصول إلى البيانات في هذه الورقة"
type: docs
url: /ar/net/aspose.cells/worksheet/startaccesscache/
---
## Worksheet.StartAccessCache method

يبدأ الجلسة التي تستخدم الذاكرة المؤقتة للوصول إلى البيانات في هذه ورقة العمل.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| opts | AccessCacheOptions | خيارات الوصول إلى البيانات |

### ملاحظات

بعد الانتهاء من الوصول إلى البيانات، يجب استدعاء [`CloseAccessCache`](../closeaccesscache/) بنفس الخيارات لمسح جميع الذاكرات المؤقتة واستعادة وضع الوصول العادي.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodStartAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // تعيين النمط الافتراضي
            Style style = wb.DefaultStyle;
            style.Font.Size = 10;
            wb.DefaultStyle = style;

            // إضافة تنسيق شرطي
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 10, 10));
            fcc.AddCondition(FormatConditionType.DuplicateValues);
            FormatCondition fc = fcc[0];
            fc.Style.Font.Size = 16;

            // ملء بعض البيانات
            Cells cells = sheet.Cells;
            for (int i = 0; i < 10; i++)
            {
                cells[0, i].PutValue("A");
                cells[i, 0].PutValue(i);
            }

            // ابدأ ذاكرة الوصول المؤقت لتحسين الأداء
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // تحقق من الأنماط
            for (int i = 0; i < 10; i++)
            {
                Console.WriteLine($"Cell[0,{i}] Font Size: {cells[0, i].GetDisplayStyle().Font.Size}");
                Console.WriteLine($"Cell[{i},0] Font Size: {cells[i, 0].GetDisplayStyle().Font.Size}");
            }

            // إغلاق الذاكرة المؤقتة عند الانتهاء
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


