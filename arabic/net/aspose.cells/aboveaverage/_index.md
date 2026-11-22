---
title: "الفئة AboveAverage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.AboveAverage. صِف قاعدة تنسيق الخلايا الشرطية AboveAverage. تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تكون أعلى أو أقل من المتوسط لجميع القيم في النطاق"
type: docs
url: /ar/net/aspose.cells/aboveaverage/
---
## AboveAverage class

صف قاعدة تنسيق الخلايا الشرطية AboveAverage. تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تكون فوق أو تحت المتوسط لجميع القيم في النطاق.

```csharp
public class AboveAverage
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [AboveAverage](aboveaverage/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [IsAboveAverage](../../aspose.cells/aboveaverage/isaboveaverage/) { get; set; } | احصل أو اضبط العلامة التي تشير إلى ما إذا كانت القاعدة قاعدة "متوسط أعلى". 'true' يعني 'متوسط أعلى'. القيمة الافتراضية هي true. |
| [IsEqualAverage](../../aspose.cells/aboveaverage/isequalaverage/) { get; set; } | احصل أو اضبط العلامة التي تشير إلى ما إذا كانت معايير 'aboveAverage' و 'belowAverage' تشمل المتوسط نفسه أم تستثنيه. 'true' يعني تضمين قيمة المتوسط في المعايير. القيمة الافتراضية هي false. |
| [StdDev](../../aspose.cells/aboveaverage/stddev/) { get; set; } | احصل أو اضبط عدد الانحرافات المعيارية لتضمينها أعلى أو أسفل المتوسط في قاعدة تنسيق الخلايا الشرطية. يجب أن تكون القيمة المدخلة بين 0 و 3 (تشمل 0 و 3). ضبط هذه القيمة إلى 0 يعني عدم تعيين stdDev. القيمة الافتراضية هي 0. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class AboveAverageDemo
    {
        public static void AboveAverageExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            // إضافة مجموعة تنسيق خلايا شرطية إلى ورقة العمل
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            // تحديد نطاق الخلايا لتطبيق تنسيق الخلايا الشرطية
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // إضافة شرط متوسط أعلى إلى المجموعة
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            // ضبط لون الخلفية للشرط
            fc.Style.BackgroundColor = Color.Yellow;

            // ضبط الخصائص للشرط متوسط أعلى
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            Cells cells = worksheet.Cells;
            cells["A1"].Value = 20;
            cells["A2"].Value = 300;
            cells["A3"].Value = 40;
            cells["A4"].Value = 500;
            cells["A5"].Value = 6;
            cells["A6"].Value = 70;
            cells["A7"].Value = 8;
            cells["A8"].Value = 900;
            cells["A9"].Value = 10;

            cells["C1"].Value = 2;
            cells["C2"].Value = 3;
            cells["C3"].Value = 4;
            cells["C4"].Value = 5;
            cells["C5"].Value = 3;
            cells["C6"].Value = 2;
            cells["C7"].Value = 8;
            cells["C8"].Value = 300;
            cells["C9"].Value = 10;

            // احفظ المصنف
            workbook.Save("AboveAverageExample.xlsx");
            workbook.Save("AboveAverageExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


