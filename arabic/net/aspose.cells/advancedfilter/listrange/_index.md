---
title: "AdvancedFilter.ListRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AdvancedFilter. تحصل على نطاق القائمة لهذا الفلتر المتقدم"
type: docs
url: /ar/net/aspose.cells/advancedfilter/listrange/
---
## AdvancedFilter.ListRange property

يحصل على نطاق القائمة لهذا الفلتر المتقدم.

```csharp
public string ListRange { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AdvancedFilterPropertyListRangeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // ملء بيانات عينة
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Person " + (i-1));
                sheet.Cells["B" + i].PutValue(20 + i);
            }

            // إعداد الفلتر المتقدم
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            // ListRange للقراءة فقط ويتم تعيينه تلقائيًا عند إنشاء الفلتر
            // يمكننا فقط قراءته، وليس تعيينه مباشرة
            
            // عرض نطاق القائمة (سيظهر النطاق المحدد تلقائيًا)
            Console.WriteLine("Advanced Filter List Range: " + filter.ListRange);
            
            // احفظ المصنف
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


