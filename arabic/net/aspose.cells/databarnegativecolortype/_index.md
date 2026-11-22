---
title: "تعداد DataBarNegativeColorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.DataBarNegativeColorType. يحدد ما إذا كان يجب استخدام نفس لون الحدود والملء مثل أشرطة البيانات الإيجابية"
type: docs
url: /ar/net/aspose.cells/databarnegativecolortype/
---
## DataBarNegativeColorType enumeration

يحدد ما إذا كان سيتم استخدام نفس لون الحدود والتعبئة كأشرطة البيانات الإيجابية.

```csharp
public enum DataBarNegativeColorType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Color | `0` | استخدم اللون المحدد في مربع حوار القيمة السلبية وإعداد المحور أو باستخدام خصائص ColorType و BorderColorType لكائن NegativeBarFormat. |
| SameAsPositive | `1` | استخدم نفس اللون مثل أشرطة البيانات الإيجابية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarNegativeColorTypeDemo
    {
        public static void DataBarNegativeColorTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(-20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(-40);
            worksheet.Cells["A5"].PutValue(50);

            // إضافة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // تعيين خصائص شريط البيانات
            DataBar dataBar = fc.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Number;
            dataBar.MinCfvo.Value = -50;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Number;
            dataBar.MaxCfvo.Value = 50;
            dataBar.Color = System.Drawing.Color.Green;

            // تعيين خصائص تنسيق الشريط السلبي
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = System.Drawing.Color.Red;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = System.Drawing.Color.Blue;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.SameAsPositive;

            // احفظ المصنف
            workbook.Save("DataBarNegativeColorTypeExample.xlsx");
            workbook.Save("DataBarNegativeColorTypeExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


