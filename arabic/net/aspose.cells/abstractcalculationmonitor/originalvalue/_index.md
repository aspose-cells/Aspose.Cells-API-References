---
title: "AbstractCalculationMonitor.OriginalValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AbstractCalculationMonitor. تحصل على القيمة القديمة للخلية المحسوبة. يجب استخدامها فقط في BeforeCalculate و AfterCalculate"
type: docs
url: /ar/net/aspose.cells/abstractcalculationmonitor/originalvalue/
---
## AbstractCalculationMonitor.OriginalValue property

تحصل على القيمة القديمة للخلية المحسوبة. يجب استخدامها فقط في [`BeforeCalculate`](../beforecalculate/) و [`AfterCalculate`](../aftercalculate/).

```csharp
public object OriginalValue { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomCalculationMonitor1 : AbstractCalculationMonitor
    {
        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            if (ValueChanged)
            {
                Console.WriteLine($"Value changed from [{OriginalValue}] to [{CalculatedValue}]");
            }
        }
    }

    public class AbstractCalculationMonitorPropertyOriginalValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين القيمة الأولية
            worksheet.Cells["A1"].PutValue(10);
            
            // إضافة صيغة ستغير القيمة
            worksheet.Cells["A2"].Formula = "=A1*2";
            
            // تعيين مراقب الحساب
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CustomCalculationMonitor1();
            
            // إعادة حساب الصيغ - سيؤدي ذلك إلى تشغيل المراقب
            workbook.CalculateFormula(options);
            
            // تغيير القيمة الأصلية لتوضيح عمل المراقب
            worksheet.Cells["A1"].PutValue(20);
            workbook.CalculateFormula(options);
        }
    }
}
```

### انظر أيضًا

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


