---
title: "FormatCondition.DataBar"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormatCondition. احصل على نسخة DataBar من تنسيقات الشرطية. اللون الافتراضي للنسخة هو الأزرق. صالح فقط للنوع DataBar"
type: docs
url: /ar/net/aspose.cells/formatcondition/databar/
---
## FormatCondition.DataBar property

احصل على نسخة "DataBar" من تنسيق الشرطي. لون النسخة الافتراضية هو الأزرق. صالحة فقط للنوع هو DataBar.

```csharp
public DataBar DataBar { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyDataBarDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // إضافة تنسيق شرطي لشريط البيانات
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // حدد النطاق للتنسيق الشرطي
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // أضف شرط شريط البيانات واضبط الخصائص
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = fcs[conditionIndex];
            
            // تكوين خصائص DataBar
            DataBar dataBar = condition.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            dataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            dataBar.Color = System.Drawing.Color.Green;

            // احفظ المصنف
            workbook.Save("DataBarExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataBar](../../databar/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


