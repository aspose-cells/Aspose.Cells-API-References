---
title: "CellsHelper.SignificantDigits"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsHelper. تحصل أو تعين عدد الأرقام ذات الدقة. القيمة الافتراضية هي 17"
type: docs
url: /ar/net/aspose.cells/cellshelper/significantdigits/
---
## CellsHelper.SignificantDigits property

يحصل أو يعين عدد الأرقام ذات الدقة. القيمة الافتراضية هي 17.

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static int SignificantDigits { get; set; }
```

### ملاحظات

يمكن أن يكون الآن 15 أو 17 فقط. ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام [`SignificantDigitsType`](../significantdigitstype/). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // عيّن الأرقام ذات الدقة
            CellsHelper.SignificantDigits = 15;
            
            // أظهر استخدام الخاصية
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            
            // أنشئ دفتر عمل لإظهار الأرقام ذات الدقة في الحسابات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // عيّن القيم التي سيتأثر بها الأرقام ذات الدقة
            worksheet.Cells["A1"].PutValue(1.2345678912345678);
            worksheet.Cells["A2"].PutValue(1.2345678912345678);
            worksheet.Cells["A3"].Formula = "=A1+A2";
            
            // احسب الصيغ باستخدام الأرقام ذات الدقة المحددة
            workbook.CalculateFormula();
            
            // أخرج النتائج
            Console.WriteLine("Value with significant digits: " + worksheet.Cells["A3"].Value);
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


