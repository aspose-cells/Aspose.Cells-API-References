---
title: "CellsHelper.SignificantDigitsType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsHelper. تحصل وتضبط النوع الافتراضي للأرقام ذات الأهمية عند إخراج القيم الرقمية. القيمة الافتراضية هي G17"
type: docs
url: /ar/net/aspose.cells/cellshelper/significantdigitstype/
---
## CellsHelper.SignificantDigitsType property

يحصل ويعيّن النوع الافتراضي للأرقام ذات الدقة لإخراج القيم الرقمية. القيمة الافتراضية هي G17.

```csharp
public static SignificantDigitsType SignificantDigitsType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // اعرض قيمة SignificantDigitsType الحالية
                Console.WriteLine("Current SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // اضبط قيمة جديدة لـ SignificantDigitsType
                CellsHelper.SignificantDigitsType = SignificantDigitsType.G17;
                Console.WriteLine("Updated SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // أنشئ دفتر عمل لتوضيح التأثير
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // أضف قيمة رقمية ستتأثر بالأرقام ذات الأهمية
                worksheet.Cells["A1"].PutValue(1.2345678912345678);
                worksheet.Cells["A2"].PutValue(1.2345678912345678);
                worksheet.Cells["A3"].Formula = "=A1+A2";

                // احسب الصيغ باستخدام نوع الأرقام ذات الأهمية الحالي
                workbook.CalculateFormula();

                // اعرض النتيجة
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].Value);

                // غيّر إلى نوع آخر من الأرقام ذات الأهمية
                CellsHelper.SignificantDigitsType = SignificantDigitsType.Rounding17;
                Console.WriteLine("Changed SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // أعد الحساب باستخدام نوع الأرقام ذات الأهمية الجديد
                workbook.CalculateFormula();
                Console.WriteLine("Recalculated result: " + worksheet.Cells["A3"].Value);

                // احفظ المصنف
                workbook.Save("SignificantDigitsTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


