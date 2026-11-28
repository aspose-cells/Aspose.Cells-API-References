---
title: "AbstractCalculationMonitor.OriginalValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractCalculationMonitor özelliği. Hesaplanan hücrenin eski değerini alır. Yalnızca BeforeCalculate ve AfterCalculate içinde kullanılmalıdır."
type: docs
url: /tr/net/aspose.cells/abstractcalculationmonitor/originalvalue/
---
## AbstractCalculationMonitor.OriginalValue property

Hesaplanan hücrenin eski değerini alır. Yalnızca [`BeforeCalculate`](../beforecalculate/) ve [`AfterCalculate`](../aftercalculate/) içinde kullanılmalıdır.

```csharp
public object OriginalValue { get; }
```

### Örnekler

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

            // İlk değeri ayarlayın
            worksheet.Cells["A1"].PutValue(10);
            
            // Değeri değiştirecek formülü ekleyin
            worksheet.Cells["A2"].Formula = "=A1*2";
            
            // Hesaplama monitörünü ayarlayın
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CustomCalculationMonitor1();
            
            // Formülleri yeniden hesaplayın - bu monitörü tetikleyecek
            workbook.CalculateFormula(options);
            
            // Monitörü göstermek için orijinal değeri değiştirin
            worksheet.Cells["A1"].PutValue(20);
            workbook.CalculateFormula(options);
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


