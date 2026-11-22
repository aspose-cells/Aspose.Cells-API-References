---
title: "AboveAverage.IsEqualAverage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AboveAverage. الحصول أو ضبط العلامة التي تشير إلى ما إذا كان معيار فوق المتوسط وتحت المتوسط شاملًا للمتوسط نفسه أو مستثنىً من تلك القيمة. true يدل على تضمين قيمة المتوسط في المعيار. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/aboveaverage/isequalaverage/
---
## AboveAverage.IsEqualAverage property

احصل أو اضبط العلامة التي تشير إلى ما إذا كانت معايير 'aboveAverage' و 'belowAverage' تشمل المتوسط نفسه أم تستثنيه. 'true' يعني تضمين قيمة المتوسط في المعايير. القيمة الافتراضية هي false.

```csharp
public bool IsEqualAverage { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyIsEqualAverageDemo
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
            fc.Style.BackgroundColor = Color.LightBlue;

            // عرض خاصية IsEqualAverage
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false; // Cells equal to average won't be formatted

            // ملء بيانات عينة
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            worksheet.Cells["A4"].Value = 40;
            worksheet.Cells["A5"].Value = 50; // Average is 30

            workbook.Save("AboveAverageIsEqualAverageDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


