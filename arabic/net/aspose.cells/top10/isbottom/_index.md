---
title: "Top10.IsBottom"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Top10. الحصول أو الضبط ما إذا كانت قاعدة أعلى/أسفل n هي قاعدة أسفل n. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/top10/isbottom/
---
## Top10.IsBottom property

احصل أو عيّن ما إذا كانت قاعدة "top/bottom n" هي قاعدة "bottom n". القيمة الافتراضية هي false.

```csharp
public bool IsBottom { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class Top10PropertyIsBottomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i + 1);
            }

            // إضافة تنسيق شرطي
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            fcs.AddArea(new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 0 });

            // إضافة شرط Top10
            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // تكوين خصائص Top10
            Top10 top10 = fc.Top10;
            top10.IsBottom = true; // Highlight bottom values
            top10.IsPercent = false;
            top10.Rank = 3; // Highlight bottom 3 values

            workbook.Save("Top10IsBottomExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


