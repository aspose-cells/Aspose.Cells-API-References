---
title: "AbstractCalculationMonitor.ValueChanged"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AbstractCalculationMonitor. ما إذا تم تغيير قيمة الخلية بعد الحساب. يجب استخدامها فقط في AfterCalculate"
type: docs
url: /ar/net/aspose.cells/abstractcalculationmonitor/valuechanged/
---
## AbstractCalculationMonitor.ValueChanged property

ما إذا تم تغيير قيمة الخلية بعد الحساب. يجب استخدامها فقط في [`AfterCalculate`](../aftercalculate/).

```csharp
public bool ValueChanged { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomCalculationMonitor2 : AbstractCalculationMonitor
    {
        public bool Changed { get; set; }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            if (ValueChanged)
            {
                Changed = true;
                Console.WriteLine($"Value changed from [{OriginalValue}] to [{CalculatedValue}]");
            }
        }
    }

    public class AbstractCalculationMonitorPropertyValueChangedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين القيمة الأولية
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Formula = "=A1*2";

            // إنشاء وتعيين مراقب الحساب
            CustomCalculationMonitor2 monitor = new CustomCalculationMonitor2();
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = monitor;

            // الحساب الأول
            workbook.CalculateFormula(options);
            Console.WriteLine($"First calculation - Changed: {monitor.Changed}");

            // تغيير القيمة وإعادة الحساب
            worksheet.Cells["A1"].Value = 20;
            monitor.Changed = false;
            workbook.CalculateFormula(options);
            Console.WriteLine($"Second calculation - Changed: {monitor.Changed}");
        }
    }
}
```

### انظر أيضًا

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


