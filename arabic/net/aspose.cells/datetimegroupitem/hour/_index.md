---
title: "DateTimeGroupItem.Hour"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DateTimeGroupItem. تحصل وتضبط ساعة التاريخ والوقت المجمع"
type: docs
url: /ar/net/aspose.cells/datetimegroupitem/hour/
---
## DateTimeGroupItem.Hour property

يحصل على ساعة التاريخ والوقت المجمّع ويضبطها.

```csharp
public int Hour { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyHourDemo
    {
        public static void Run()
        {
            // إنشاء DateTimeGroupItem مع تجميع حسب الساعة
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Hour,
                2023,  // Year
                10,     // Month
                5,      // Day
                14,     // Hour
                0,      // Minute
                0      // Second
            );

            // عرض قيمة الساعة الأولية
            Console.WriteLine("Initial Hour: " + dateTimeGroupItem.Hour);

            // تعديل خاصية الساعة
            dateTimeGroupItem.Hour = 18;

            // عرض قيمة الساعة المعدلة
            Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
        }
    }
}
```

### انظر أيضًا

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


