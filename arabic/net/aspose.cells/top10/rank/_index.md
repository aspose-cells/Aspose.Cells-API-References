---
title: "Top10.Rank"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Top10. الحصول على قيمة n أو تعيينها في قاعدة تنسيق شرطي أعلى/أسفل n. إذا كان IsPercent صحيحًا يجب أن تكون القيمة بين 0 و 100. وإلا يجب أن تكون بين 0 و 1000. القيمة الافتراضية هي 10"
type: docs
url: /ar/net/aspose.cells/top10/rank/
---
## Top10.Rank property

احصل أو عيّن قيمة "n" في قاعدة التنسيق الشرطي "top/bottom n". إذا كان IsPercent صحيحًا، يجب أن تكون القيمة بين 0 و 100. وإلا يجب أن تكون بين 0 و 1000. القيمة الافتراضية هي 10.

```csharp
public int Rank { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class Top10PropertyRankDemo
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
            top10.Rank = 5;

            workbook.Save("Top10RankExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


