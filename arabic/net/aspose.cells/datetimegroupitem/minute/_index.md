---
title: "DateTimeGroupItem.Minute"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DateTimeGroupItem. تحصل وتضبط الدقيقة لتاريخ الوقت المجمع"
type: docs
url: /ar/net/aspose.cells/datetimegroupitem/minute/
---
## DateTimeGroupItem.Minute property

يحصل على دقيقة التاريخ والوقت المجمّع ويضبطها.

```csharp
public int Minute { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMinuteDemo
    {
        public static void Run()
        {
            // إنشاء DateTimeGroupItem بقيم أولية
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                10,
                5,
                14,
                30,
                45
            );

            // عرض قيمة الدقيقة الأولية
            Console.WriteLine("Initial Minute: " + dateTimeGroupItem.Minute);

            // تغيير قيمة الدقيقة
            dateTimeGroupItem.Minute = 15;

            // عرض قيمة الدقيقة المعدلة
            Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);

            // إنشاء DateTimeGroupItem جديد مع تجميع دقيقة فقط
            DateTimeGroupItem minuteGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Minute,
                0, 0, 0, 0, 45, 0
            );

            // عرض الدقيقة من تجميع الدقيقة
            Console.WriteLine("Minute from Minute Grouping: " + minuteGroup.Minute);
        }
    }
}
```

### انظر أيضًا

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


