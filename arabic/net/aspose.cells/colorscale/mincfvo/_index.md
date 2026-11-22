---
title: "ColorScale.MinCfvo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ColorScale. احصل أو عيّن كائن القيمة الدنيا لهذا ColorScales. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Max إليه"
type: docs
url: /ar/net/aspose.cells/colorscale/mincfvo/
---
## ColorScale.MinCfvo property

احصل أو عيّن كائن القيمة الدنيا لهذا ColorScale. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Max إليه.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMinCfvoDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // أنشئ تنسيقًا شرطيًا لمقياس اللون
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // أضف مقياس لون
            int csIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            ColorScale cs = fcc[csIndex].ColorScale;

            // عيّن خصائص MinCfvo
            cs.MinCfvo.Type = FormatConditionValueType.Min;
            cs.MinCfvo.Value = "0";
            cs.MinColor = System.Drawing.Color.Red;

            // عيّن خصائص MidCfvo
            cs.MidCfvo.Type = FormatConditionValueType.Percentile;
            cs.MidCfvo.Value = "50";
            cs.MidColor = System.Drawing.Color.Yellow;

            // عيّن خصائص MaxCfvo
            cs.MaxCfvo.Type = FormatConditionValueType.Max;
            cs.MaxCfvo.Value = "0";
            cs.MaxColor = System.Drawing.Color.Green;

            // احفظ المصنف
            workbook.Save("ColorScaleMinCfvoDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


