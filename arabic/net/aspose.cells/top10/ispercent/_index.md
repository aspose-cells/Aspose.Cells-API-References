---
title: "Top10.IsPercent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Top10. الحصول أو الضبط ما إذا كانت قاعدة أعلى/أسفل n هي قاعدة أعلى/أسفل n بالنسبة المئوية. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/top10/ispercent/
---
## Top10.IsPercent property

احصل أو عيّن ما إذا كانت قاعدة "top/bottom n" هي قاعدة "top/bottom n percent". القيمة الافتراضية هي false.

```csharp
public bool IsPercent { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10PropertyIsPercentDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // إضافة قاعدة تنسيق شرطي Top10
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.Top10, OperatorType.None, null, null);

            // احصل على شرط تنسيق Top10
            FormatCondition fc = fcc[0];
            
            // تعيين خصائص Top10
            fc.Top10.IsPercent = true;  // Demonstrate IsPercent property
            fc.Top10.IsBottom = false;
            fc.Top10.Rank = 3;

            // تطبيق نمط التنسيق
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // احفظ المصنف
            workbook.Save("Top10IsPercentDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


