---
title: "DateTimeGroupItem.Month"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DateTimeGroupItem. تحصل وتضبط الشهر لتاريخ الوقت المجمع"
type: docs
url: /ar/net/aspose.cells/datetimegroupitem/month/
---
## DateTimeGroupItem.Month property

يحصل على شهر التاريخ والوقت المجمّع ويضبطه.

```csharp
public int Month { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMonthDemo
    {
        public static void Run()
        {
            // إنشاء DateTimeGroupItem مجمع حسب Month
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Month,
                2023,
                10,
                1,
                0,
                0,
                0
            );

            // عرض قيمة الشهر الأولية
            Console.WriteLine("Initial Month: " + dateTimeGroupItem.Month);

            // تغيير قيمة الشهر
            dateTimeGroupItem.Month = 12;
            Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);

            // إنشاء DateTimeGroupItem آخر مع تجميع مختلف
            DateTimeGroupItem yearlyItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                1,
                1,
                0,
                0,
                0
            );

            // إظهار أن خاصية Month لا تزال قابلة للوصول حتى عند التجميع حسب Year
            Console.WriteLine("Yearly Grouping - Month: " + yearlyItem.Month);
        }
    }
}
```

### انظر أيضًا

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


