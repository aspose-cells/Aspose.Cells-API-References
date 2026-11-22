---
title: "DateTimeGroupItem.Year"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DateTimeGroupItem. يحصل على السنة ويضبطها لتاريخ الوقت المجمع"
type: docs
url: /ar/net/aspose.cells/datetimegroupitem/year/
---
## DateTimeGroupItem.Year property

يحصل على سنة التاريخ والوقت المجمّع ويضبطها.

```csharp
public int Year { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyYearDemo
    {
        public static void Run()
        {
            // إنشاء DateTimeGroupItem مجمّع حسب السنة
            DateTimeGroupItem dateTimeGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                1,     // Month (ignored when grouping by Year)
                1,     // Day (ignored)
                0,     // Hour (ignored)
                0,     // Minute (ignored)
                0      // Second (ignored)
            );

            // عرض قيمة السنة الأولية
            Console.WriteLine("Initial Year: " + dateTimeGroup.Year);

            // تعديل خاصية السنة
            dateTimeGroup.Year = 2024;

            // عرض قيمة السنة المعدلة
            Console.WriteLine("Modified Year: " + dateTimeGroup.Year);

            // إظهار أن الخصائص الأخرى يتم تجاهلها عند التجميع حسب السنة
            dateTimeGroup.Month = 12;
            Console.WriteLine("Month value is ignored when grouping by Year: " + dateTimeGroup.Month);
        }
    }
}
```

### انظر أيضًا

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


