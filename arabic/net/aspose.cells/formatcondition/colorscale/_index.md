---
title: "FormatCondition.ColorScale"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormatCondition. احصل على مثيل ColorScale للتنسيقات الشرطية. المثيل الافتراضي هو 3ColorScale باللون الأخضر الأصفر الأحمر. صالح فقط للنوع ColorScale"
type: docs
url: /ar/net/aspose.cells/formatcondition/colorscale/
---
## FormatCondition.ColorScale property

احصل على نسخة "ColorScale" من تنسيق الشرطي. النسخة الافتراضية هي "green-yellow-red" 3ColorScale. صالحة فقط للنوع = ColorScale.

```csharp
public ColorScale ColorScale { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyColorScaleDemo
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

            // أضف تنسيقًا شرطيًا لمقياس اللون
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // تعيين النطاق للتنسيق الشرطي
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // تعيين خصائص مقياس اللون
            fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[0];
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Green;

            // احفظ المصنف
            workbook.Save("ColorScaleExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ColorScale](../../colorscale/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


