---
title: "AbstractCalculationMonitor.ValueChanged"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractCalculationMonitor özelliği. Hesaplamadan sonra hücrenin değerinin değişip değişmediği. Yalnızca AfterCalculate içinde kullanılmalıdır."
type: docs
url: /tr/net/aspose.cells/abstractcalculationmonitor/valuechanged/
---
## AbstractCalculationMonitor.ValueChanged property

Hesaplamadan sonra hücrenin değerinin değişip değişmediği. Yalnızca [`AfterCalculate`](../aftercalculate/) içinde kullanılmalıdır.

```csharp
public bool ValueChanged { get; }
```

### Örnekler

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

            // İlk değeri ayarlayın
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Formula = "=A1*2";

            // Hesaplama monitörünü oluşturun ve ayarlayın
            CustomCalculationMonitor2 monitor = new CustomCalculationMonitor2();
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = monitor;

            // İlk hesaplama
            workbook.CalculateFormula(options);
            Console.WriteLine($"First calculation - Changed: {monitor.Changed}");

            // Değeri değiştir ve yeniden hesapla
            worksheet.Cells["A1"].Value = 20;
            monitor.Changed = false;
            workbook.CalculateFormula(options);
            Console.WriteLine($"Second calculation - Changed: {monitor.Changed}");
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


