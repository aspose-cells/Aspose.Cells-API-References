---
title: "DateTimeGroupItem.Day"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DateTimeGroupItem. تحصل وتضبط اليوم لتاريخ الوقت المجمع"
type: docs
url: /ar/net/aspose.cells/datetimegroupitem/day/
---
## DateTimeGroupItem.Day property

يحصل على يوم التاريخ والوقت المجمّع ويضبطه.

```csharp
public int Day { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyDayDemo
    {
        public static void Run()
        {
            // إنشاء DateTimeGroupItem مجمّع حسب السنة
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                10,    // Month
                5,     // Day
                14,    // Hour
                30,    // Minute
                45     // Second
            );

            // عرض قيمة اليوم الأولية
            Console.WriteLine("Initial Day: " + dateTimeGroupItem.Day);

            // تغيير خاصية اليوم
            dateTimeGroupItem.Day = 25;
            Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);

            // إنشاء DateTimeGroupItem آخر مجمع حسب Day لتوضيح أهمية خاصية Day
            DateTimeGroupItem dayGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Day,
                2023,
                10,
                15,  // Initial day
                0,
                0,
                0
            );

            Console.WriteLine("\nDay-grouped item initial Day: " + dayGroupItem.Day);
            dayGroupItem.Day = 20;
            Console.WriteLine("Day-grouped item modified Day: " + dayGroupItem.Day);
        }
    }
}
```

### انظر أيضًا

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


