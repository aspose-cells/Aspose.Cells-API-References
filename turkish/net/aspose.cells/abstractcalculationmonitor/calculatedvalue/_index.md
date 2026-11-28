---
title: "AbstractCalculationMonitor.CalculatedValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractCalculationMonitor özelliği. Hücrenin yeni hesaplanan değerini alır. Yalnızca AfterCalculate içinde kullanılmalıdır."
type: docs
url: /tr/net/aspose.cells/abstractcalculationmonitor/calculatedvalue/
---
## AbstractCalculationMonitor.CalculatedValue property

Hücrenin yeni hesaplanan değerini alır. Yalnızca [`AfterCalculate`](../aftercalculate/) içinde kullanılmalıdır.

```csharp
public object CalculatedValue { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomCalculationMonitor : AbstractCalculationMonitor
    {
        public override void AfterCalculate(int sheetIndex, int rowIndex, int columnIndex)
        {
            if (ValueChanged)
            {
                Console.WriteLine($"Value changed from [{OriginalValue}] to [{CalculatedValue}]");
            }
        }
    }

    public class AbstractCalculationMonitorPropertyCalculatedValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hesaplama zincirini kurun
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";

            // Monitörü oluşturun ve ekleyin
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = monitor;

            // Monitörümüzü çağıracak hesaplamayı tetikleyin
            workbook.CalculateFormula(options);

            // Değişiklik bildirimi tetiklemek için bir değeri değiştirin
            worksheet.Cells["A1"].Value = 5;
            workbook.CalculateFormula(options);
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


