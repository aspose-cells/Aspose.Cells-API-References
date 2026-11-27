---
title: "AbstractCalculationMonitor.OriginalValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractCalculationMonitor-egenskap. Hämtar det gamla värdet för den beräknade cellen. Bör endast användas i BeforeCalculate och AfterCalculate"
type: docs
url: /sv/net/aspose.cells/abstractcalculationmonitor/originalvalue/
---
## AbstractCalculationMonitor.OriginalValue property

Hämtar det gamla värdet för den beräknade cellen. Bör endast användas i [`BeforeCalculate`](../beforecalculate/) och [`AfterCalculate`](../aftercalculate/).

```csharp
public object OriginalValue { get; }
```

### Exempel

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

            // Ange initialt värde
            worksheet.Cells["A1"].PutValue(10);
            
            // Lägg till formel som kommer att ändra värdet
            worksheet.Cells["A2"].Formula = "=A1*2";
            
            // Ställ in beräkningsmonitor
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CustomCalculationMonitor1();
            
            // Beräkna om formler - detta kommer att trigga monitorn
            workbook.CalculateFormula(options);
            
            // Ändra det ursprungliga värdet för att demonstrera monitorn
            worksheet.Cells["A1"].PutValue(20);
            workbook.CalculateFormula(options);
        }
    }
}
```

### Se även

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


