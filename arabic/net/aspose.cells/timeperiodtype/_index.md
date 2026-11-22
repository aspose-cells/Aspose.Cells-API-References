---
title: "التعداد TimePeriodType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.TimePeriodType. يُستخدم في قاعدة تنسيق شرطي FormatConditionType.TimePeriod. هذه فترات زمنية ديناميكية تتغير بناءً على تاريخ تحديث / تطبيق التنسيق الشرطي"
type: docs
url: /ar/net/aspose.cells/timeperiodtype/
---
## TimePeriodType enumeration

يُستخدم في قاعدة تنسيق شرطي من النوع FormatConditionType.TimePeriod. هذه فترات زمنية ديناميكية، تتغير بناءً على تاريخ تحديث / تطبيق التنسيق الشرطي.

```csharp
public enum TimePeriodType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Today | `0` | تاريخ اليوم. |
| Yesterday | `1` | تاريخ الأمس. |
| Tomorrow | `2` | تاريخ الغد. |
| Last7Days | `3` | تاريخ ضمن الأيام السبعة الأخيرة. |
| ThisMonth | `4` | تاريخ يحدث في هذا الشهر التقويمي. |
| LastMonth | `5` | تاريخ يحدث في الشهر التقويمي الأخير. |
| NextMonth | `6` | تاريخ يحدث في الشهر التقويمي التالي. |
| ThisWeek | `7` | تاريخ يحدث هذا الأسبوع. |
| LastWeek | `8` | تاريخ يحدث الأسبوع الماضي. |
| NextWeek | `9` | تاريخ يحدث الأسبوع القادم. |
| ThisYear | `10` | تاريخ يحدث هذا العام. فقط لملفات .ods. |
| LastYear | `11` | تاريخ يحدث العام الماضي. فقط لملفات .ods. |
| NextYear | `12` | تاريخ يحدث العام القادم. فقط لملفات .ods. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TimePeriodTypeDemo
    {
        public static void TimePeriodTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة قاعدة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // تحديد نطاق الخلايا للتنسيق الشرطي
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // إضافة شرط لفترة الوقت
            int conditionIndex = fcs.AddCondition(FormatConditionType.TimePeriod);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.LightBlue;

            // تعيين نوع فترة الوقت
            fc.TimePeriod = TimePeriodType.Today;

            // احفظ المصنف
            workbook.Save("TimePeriodTypeExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


