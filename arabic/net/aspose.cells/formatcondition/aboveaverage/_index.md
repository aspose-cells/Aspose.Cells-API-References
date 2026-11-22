---
title: "FormatCondition.AboveAverage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormatCondition. احصل على نسخة AboveAverage من تنسيقات الشرطية. القاعدة الافتراضية للنسخة تبرز الخلايا التي تكون فوق المتوسط لجميع القيم في النطاق. صالح فقط للنوع AboveAverage"
type: docs
url: /ar/net/aspose.cells/formatcondition/aboveaverage/
---
## FormatCondition.AboveAverage property

احصل على نسخة "AboveAverage" من تنسيق الشرطي. القاعدة الافتراضية للنسخة تبرز الخلايا التي تكون فوق المتوسط لجميع القيم في النطاق. صالحة فقط للنوع = AboveAverage.

```csharp
public AboveAverage AboveAverage { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyAboveAverageDemo
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

            // أضف تنسيقًا شرطيًا فوق المتوسط
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 4, EndColumn = 0 });

            // اضبط لتسليط الضوء على القيم فوق المتوسط
            FormatCondition fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = true;
            fc.Style.BackgroundColor = Color.Yellow;

            // أضف تنسيقًا شرطيًا تحت المتوسط
            index = worksheet.ConditionalFormattings.Add();
            fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 1, EndRow = 4, EndColumn = 1 });

            // اضبط لتسليط الضوء على القيم تحت المتوسط
            fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = false;
            fc.Style.BackgroundColor = Color.LightBlue;

            // احفظ المصنف
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AboveAverage](../../aboveaverage/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


