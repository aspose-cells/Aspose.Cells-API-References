---
title: "AboveAverage.IsAboveAverage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AboveAverage. الحصول أو ضبط العلامة التي تشير إلى ما إذا كانت القاعدة قاعدة فوق المتوسط. true يدل على فوق المتوسط. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/aboveaverage/isaboveaverage/
---
## AboveAverage.IsAboveAverage property

احصل أو اضبط العلامة التي تشير إلى ما إذا كانت القاعدة قاعدة "متوسط أعلى". 'true' يعني 'متوسط أعلى'. القيمة الافتراضية هي true.

```csharp
public bool IsAboveAverage { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyIsAboveAverageDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد
            Workbook workbook = new Workbook();
            
            // احصل على ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لعرض التنسيق الشرطي
            for (int i = 0; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // إضافة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // تحديد نطاق التنسيق الشرطي
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // إضافة شرط AboveAverage
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // تكوين خصائص AboveAverage
            fc.AboveAverage.IsAboveAverage = true;  // Highlight values above average
            fc.AboveAverage.IsEqualAverage = false; // Exclude values equal to average

            // احفظ ملف Excel
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


