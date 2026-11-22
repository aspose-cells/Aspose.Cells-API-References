---
title: "الفئة ColorScale"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ColorScale. صِف قاعدة تنسيق الخلايا الشرطي ColorScale. تنشئ قاعدة التنسيق الشرطي هذه مقياس ألوان متدرج على الخلايا"
type: docs
url: /ar/net/aspose.cells/colorscale/
---
## ColorScale class

وصف قاعدة تنسيق الخلايا الشرطي ColorScale. هذه القاعدة تنشئ مقياس ألوان متدرج على الخلايا.

```csharp
public class ColorScale
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Is3ColorScale](../../aspose.cells/colorscale/is3colorscale/) { get; set; } | يشير إلى ما إذا كان تنسيق الخلايا الشرطي مقياس ألوان ثلاثي. |
| [MaxCfvo](../../aspose.cells/colorscale/maxcfvo/) { get; } | احصل أو عيّن كائن القيمة القصوى لهذا ColorScale. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Min إليه. |
| [MaxColor](../../aspose.cells/colorscale/maxcolor/) { get; set; } | احصل أو عيّن لون التدرج للقيمة القصوى في النطاق. |
| [MidCfvo](../../aspose.cells/colorscale/midcfvo/) { get; } | احصل أو عيّن كائن القيمة المتوسطة لهذا ColorScale. لا يمكن تعيين CFValueObject من النوع FormatConditionValueType.Max أو FormatConditionValueType.Min إليه. |
| [MidColor](../../aspose.cells/colorscale/midcolor/) { get; set; } | احصل أو عيّن لون التدرج للقيمة المتوسطة في النطاق. |
| [MinCfvo](../../aspose.cells/colorscale/mincfvo/) { get; } | احصل أو عيّن كائن القيمة الدنيا لهذا ColorScale. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Max إليه. |
| [MinColor](../../aspose.cells/colorscale/mincolor/) { get; set; } | احصل أو عيّن لون التدرج للقيمة الدنيا في النطاق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColorScaleDemo
    {
        public static void ColorScaleExample()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات النموذجية إلى ورقة العمل
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i * j);
                }
            }

            // إضافة قاعدة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 9 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // الوصول إلى كائن ColorScale
            ColorScale colorScale = fc.ColorScale;

            // عيّن الخصائص لـ ColorScale
            colorScale.Is3ColorScale = true;
            colorScale.MinColor = Color.Green;
            colorScale.MidColor = Color.Yellow;
            colorScale.MaxColor = Color.Red;

            // عيّن كائنات القيمة الدنيا والمتوسطة والقصوى
            ConditionalFormattingValue minCfvo = colorScale.MinCfvo;
            minCfvo.Type = FormatConditionValueType.Min;
            minCfvo.Value = null;

            ConditionalFormattingValue midCfvo = colorScale.MidCfvo;
            midCfvo.Type = FormatConditionValueType.Percentile;
            midCfvo.Value = 50;

            ConditionalFormattingValue maxCfvo = colorScale.MaxCfvo;
            maxCfvo.Type = FormatConditionValueType.Max;
            maxCfvo.Value = null;

            // احفظ المصنف
            workbook.Save("ColorScaleExample.xlsx");
            workbook.Save("ColorScaleExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


