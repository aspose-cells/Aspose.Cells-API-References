---
title: "الفئة NegativeBarFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.NegativeBarFormat. تمثل إعدادات اللون لأشرطة البيانات للقيم السلبية التي يتم تعريفها بواسطة قاعدة تنسيق شرطي لأشرطة البيانات"
type: docs
url: /ar/net/aspose.cells/negativebarformat/
---
## NegativeBarFormat class

يمثل إعدادات اللون لأشرطة البيانات للقيم السلبية التي تم تعريفها بواسطة قاعدة تنسيق شرطي لأشرطة البيانات.

```csharp
public class NegativeBarFormat
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BorderColor](../../aspose.cells/negativebarformat/bordercolor/) { get; set; } | يحصل أو يعيّن كائن FormatColor يمكنك استخدامه لتحديد لون الحد لأشرطة البيانات السلبية. |
| [BorderColorType](../../aspose.cells/negativebarformat/bordercolortype/) { get; set; } | يشير إلى ما إذا كان يجب استخدام نفس لون الحد لأشرطة البيانات الإيجابية. |
| [Color](../../aspose.cells/negativebarformat/color/) { get; set; } | يحصل أو يعيّن كائن FormatColor يمكنك استخدامه لتحديد لون التعبئة لأشرطة البيانات السلبية. |
| [ColorType](../../aspose.cells/negativebarformat/colortype/) { get; set; } | يحصل أو يعيّن ما إذا كان يجب استخدام نفس لون التعبئة لأشرطة البيانات الإيجابية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class NegativeBarFormatDemo
    {
        public static void NegativeBarFormatExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // يضيف تنسيقًا شرطيًا فارغًا
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // يضبط نطاق التنسيق الشرطي
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // يضيف شرطًا لأشرطة البيانات
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // احصل على DataBar واضبط خصائصه
            DataBar dataBar = fc.DataBar;
            dataBar.Color = Color.Orange;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;

            // تكوين خصائص NegativeBarFormat
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = Color.White;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = Color.Yellow;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;

            // ضع بعض القيم في الخلايا
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);

            // احفظ المصنف
            workbook.Save("NegativeBarFormatExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


