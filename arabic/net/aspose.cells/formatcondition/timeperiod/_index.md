---
title: "FormatCondition.TimePeriod"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormatCondition. الفترة الزمنية المطبقة في قاعدة تنسيق شرطي لتاريخ حدوث. صالحة فقط للنوع timePeriod. القيمة الافتراضية هي TimePeriodType.Today"
type: docs
url: /ar/net/aspose.cells/formatcondition/timeperiod/
---
## FormatCondition.TimePeriod property

الفترة الزمنية القابلة للتطبيق في قاعدة تنسيق شرطي "date occurrin". صالحة فقط للنوع هو timePeriod. القيمة الافتراضية هي TimePeriodType.Today.

```csharp
public TimePeriodType TimePeriod { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTimePeriodDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة قيم تاريخية نموذجية لعرض تنسيق الفترة الزمنية
            worksheet.Cells["A1"].PutValue(DateTime.Now);
            worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-1));
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));

            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(area);

            int conditionIndex = fcs.AddCondition(FormatConditionType.TimePeriod);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.LightBlue;
            fc.TimePeriod = TimePeriodType.Today;

            workbook.Save("TimePeriodDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TimePeriodType](../../timeperiodtype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


