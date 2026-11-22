---
title: "الفئة ConditionalFormattingResult"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ConditionalFormattingResult. تمثل نتيجة التنسيق الشرطي الذي يُطبق على خلية"
type: docs
url: /ar/net/aspose.cells/conditionalformattingresult/
---
## ConditionalFormattingResult class

يمثل نتيجة تنسيق الخلايا الشرطي الذي يُطبق على خلية.

```csharp
public class ConditionalFormattingResult
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ColorScaleResult](../../aspose.cells/conditionalformattingresult/colorscaleresult/) { get; } | يحصل على لون العرض لمقياس اللون. |
| [ConditionalFormattingColorScale](../../aspose.cells/conditionalformattingresult/conditionalformattingcolorscale/) { get; } | يحصل على كائن ColorScale. |
| [ConditionalFormattingDataBar](../../aspose.cells/conditionalformattingresult/conditionalformattingdatabar/) { get; } | يحصل على كائن DataBar. |
| [ConditionalFormattingIcon](../../aspose.cells/conditionalformattingresult/conditionalformattingicon/) { get; } | يحصل على صورة مجموعة icon set. |
| [ConditionalStyle](../../aspose.cells/conditionalformattingresult/conditionalstyle/) { get; } | يحصل على نمط النتيجة الشرطية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingResultDemo
    {
        public static void ConditionalFormattingResultExample()
        {
            // إنشاء كائن مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // يضيف تنسيقًا شرطيًا فارغًا
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // يضبط نطاق التنسيق الشرطي
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // يضيف شرطًا
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // تعيين خصائص ColorScale
            fc.ColorScale.Is3ColorScale = true;
            fc.ColorScale.MinColor = Color.Red;
            fc.ColorScale.MidColor = Color.Yellow;
            fc.ColorScale.MaxColor = Color.Green;

            // تطبيق بعض القيم على الخلايا
            for (int i = 0; i <= 10; i++)
            {
                for (int j = 0; j <= 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i * j);
                }
            }

            // الحصول على نتيجة التنسيق الشرطي لخلية محددة
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult cfr = cell.GetConditionalFormattingResult();

            // الوصول إلى خصائص ConditionalFormattingResult
            Style conditionalStyle = cfr.ConditionalStyle;
            ConditionalFormattingIcon icon = cfr.ConditionalFormattingIcon;
            DataBar dataBar = cfr.ConditionalFormattingDataBar;
            ColorScale colorScale = cfr.ConditionalFormattingColorScale;
            Color colorScaleResult = cfr.ColorScaleResult;

            // عرض بعض الخصائص
            Console.WriteLine("Conditional Style Background Color: " + (conditionalStyle != null ? conditionalStyle.BackgroundColor : Color.Empty));
            Console.WriteLine("Conditional Formatting Icon Type: " + (icon != null ? icon.Type.ToString() : "No Icon"));
            Console.WriteLine("Conditional Formatting DataBar Color: " + (dataBar != null ? dataBar.Color.ToString() : "No DataBar"));
            Console.WriteLine("Conditional Formatting ColorScale Min Color: " + (colorScale != null ? colorScale.MinColor.ToString() : "No ColorScale"));
            Console.WriteLine("Color Scale Result: " + colorScaleResult);

            // احفظ المصنف
            workbook.Save("ConditionalFormattingResultExample.xlsx");
            workbook.Save("ConditionalFormattingResultExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


