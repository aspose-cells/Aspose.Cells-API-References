---
title: "ColorScale.MidCfvo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ColorScale. احصل أو عيّن كائن القيمة المتوسطة لهذا ColorScales. لا يمكن تعيين CFValueObject من النوع FormatConditionValueType.Max أو FormatConditionValueType.Min إليه"
type: docs
url: /ar/net/aspose.cells/colorscale/midcfvo/
---
## ColorScale.MidCfvo property

احصل أو عيّن كائن القيمة المتوسطة لهذا ColorScale. لا يمكن تعيين CFValueObject من النوع FormatConditionValueType.Max أو FormatConditionValueType.Min إليه.

```csharp
public ConditionalFormattingValue MidCfvo { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMidCfvoDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i * 10);
            }

            // أضف تنسيقًا شرطيًا لمقياس اللون
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            int conditionIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            
            // عيّن قيمة النقطة المتوسطة لمقياس اللون
            ColorScale colorScale = fcc[conditionIndex].ColorScale;
            colorScale.MidCfvo.Type = FormatConditionValueType.Number;
            colorScale.MidCfvo.Value = 50;

            // احفظ المصنف
            workbook.Save("ColorScalePropertyMidCfvoDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


