---
title: "AboveAverage.StdDev"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AboveAverage. الحصول أو ضبط عدد الانحرافات المعيارية لتضمينها فوق أو تحت المتوسط في قاعدة التنسيق الشرطي. يجب أن تكون القيمة المدخلة بين 0 و 3 تشمل 0 و 3. ضبط هذه القيمة إلى 0 يعني أن stdDev غير مضبوطة. القيمة الافتراضية هي 0"
type: docs
url: /ar/net/aspose.cells/aboveaverage/stddev/
---
## AboveAverage.StdDev property

احصل أو اضبط عدد الانحرافات المعيارية لتضمينها أعلى أو أسفل المتوسط في قاعدة تنسيق الخلايا الشرطية. يجب أن تكون القيمة المدخلة بين 0 و 3 (تشمل 0 و 3). ضبط هذه القيمة إلى 0 يعني عدم تعيين stdDev. القيمة الافتراضية هي 0.

```csharp
public int StdDev { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyStdDevDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            CellArea ca = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.StdDev = 2;

            // ملء بيانات عينة
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            worksheet.Cells["A4"].Value = 40;
            worksheet.Cells["A5"].Value = 50;

            workbook.Save("AboveAverageStdDevDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


