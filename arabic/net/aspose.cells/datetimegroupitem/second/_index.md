---
title: "DateTimeGroupItem.Second"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DateTimeGroupItem. يحصل ويضبط الثانية من تاريخ الوقت المجمع"
type: docs
url: /ar/net/aspose.cells/datetimegroupitem/second/
---
## DateTimeGroupItem.Second property

يحصل على ثانية التاريخ والوقت المجمّع ويضبطها.

```csharp
public int Second { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertySecondDemo
    {
        public static void Run()
        {
            // إنشاء كائن من DateTimeGroupItem
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year, // Group by Year
                2023,                      // Year
                10,                        // Month
                5,                         // Day
                14,                        // Hour
                30,                        // Minute
                45                         // Second
            );

            // عرض قيمة الثانية الأولية
            Console.WriteLine("Initial Second: " + dateTimeGroupItem.Second);

            // تعديل قيمة الثانية
            dateTimeGroupItem.Second = 50;
            Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);

            // إنشاء نسخة أخرى بقيمة ثانية مختلفة
            DateTimeGroupItem anotherItem = new DateTimeGroupItem(
                DateTimeGroupingType.Day,
                2023,
                10,
                5,
                14,
                30,
                0  // Second set to 0
            );
            Console.WriteLine("Another Item Second: " + anotherItem.Second);
        }
    }
}
```

### انظر أيضًا

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


