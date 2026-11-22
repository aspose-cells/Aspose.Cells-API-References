---
title: "الفئة DateTimeGroupItem"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.DateTimeGroupItem. تمثل إعداد مجموعة التاريخ والوقت"
type: docs
url: /ar/net/aspose.cells/datetimegroupitem/
---
## DateTimeGroupItem class

يمثل إعداد مجموعة التاريخ والوقت.

```csharp
public class DateTimeGroupItem
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [DateTimeGroupItem](datetimegroupitem/)(DateTimeGroupingType, int, int, int, int, int, int) |  |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DateTimeGroupingType](../../aspose.cells/datetimegroupitem/datetimegroupingtype/) { get; set; } | يحصل على نوع المجموعة ويضبطه. |
| [Day](../../aspose.cells/datetimegroupitem/day/) { get; set; } | يحصل على يوم التاريخ والوقت المجمّع ويضبطه. |
| [Hour](../../aspose.cells/datetimegroupitem/hour/) { get; set; } | يحصل على ساعة التاريخ والوقت المجمّع ويضبطها. |
| [Minute](../../aspose.cells/datetimegroupitem/minute/) { get; set; } | يحصل على دقيقة التاريخ والوقت المجمّع ويضبطها. |
| [MinValue](../../aspose.cells/datetimegroupitem/minvalue/) { get; } | يحصل على القيمة الدنيا. |
| [Month](../../aspose.cells/datetimegroupitem/month/) { get; set; } | يحصل على شهر التاريخ والوقت المجمّع ويضبطه. |
| [Second](../../aspose.cells/datetimegroupitem/second/) { get; set; } | يحصل على ثانية التاريخ والوقت المجمّع ويضبطها. |
| [Year](../../aspose.cells/datetimegroupitem/year/) { get; set; } | يحصل على سنة التاريخ والوقت المجمّع ويضبطها. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupItemDemo
    {
        public static void DateTimeGroupItemExample()
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

            // الوصول إلى الخصائص
            Console.WriteLine("MinValue: " + dateTimeGroupItem.MinValue);
            Console.WriteLine("DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Year: " + dateTimeGroupItem.Year);
            Console.WriteLine("Month: " + dateTimeGroupItem.Month);
            Console.WriteLine("Day: " + dateTimeGroupItem.Day);
            Console.WriteLine("Hour: " + dateTimeGroupItem.Hour);
            Console.WriteLine("Minute: " + dateTimeGroupItem.Minute);
            Console.WriteLine("Second: " + dateTimeGroupItem.Second);

            // تعديل الخصائص
            dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
            dateTimeGroupItem.Year = 2022;
            dateTimeGroupItem.Month = 12;
            dateTimeGroupItem.Day = 25;
            dateTimeGroupItem.Hour = 10;
            dateTimeGroupItem.Minute = 15;
            dateTimeGroupItem.Second = 30;

            // الوصول إلى الخصائص المعدلة
            Console.WriteLine("Modified DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Modified Year: " + dateTimeGroupItem.Year);
            Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);
            Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);
            Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
            Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);
            Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


