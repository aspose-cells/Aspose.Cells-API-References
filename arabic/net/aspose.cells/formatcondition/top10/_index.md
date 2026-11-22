---
title: "FormatCondition.Top10"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormatCondition. احصل على نسخة Top10 من تنسيقات الشرطية. القاعدة الافتراضية للنسخة تبرز الخلايا التي تقع قيمها ضمن أعلى 10 نطاقات. صالح فقط للنوع Top10"
type: docs
url: /ar/net/aspose.cells/formatcondition/top10/
---
## FormatCondition.Top10 property

احصل على نسخة "Top10" من تنسيق الشرطي. القاعدة الافتراضية للنسخة تبرز الخلايا التي تقع قيمها في أعلى 10 نطاقات. صالحة فقط للنوع هو Top10.

```csharp
public Top10 Top10 { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTop10Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            Top10 top10 = fc.Top10;
            top10.IsPercent = true;
            top10.IsBottom = true;
            top10.Rank = 10;

            workbook.Save("FormatConditionPropertyTop10Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Top10](../../top10/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


