---
title: "AbstractCalculationMonitor.ValueChanged"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractCalculationMonitor-egenskap. Anger om cellens värde har ändrats efter beräkningen. Bör endast användas i AfterCalculate"
type: docs
url: /sv/net/aspose.cells/abstractcalculationmonitor/valuechanged/
---
## AbstractCalculationMonitor.ValueChanged property

Om cellens värde har ändrats efter beräkningen. Bör endast användas i [`AfterCalculate`](../aftercalculate/).

```csharp
public bool ValueChanged { get; }
```

### Exempel

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

            // Ange initialt värde
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Formula = "=A1*2";

            // Skapa och ställ in beräkningsmonitor
            CustomCalculationMonitor2 monitor = new CustomCalculationMonitor2();
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = monitor;

            // Första beräkningen
            workbook.CalculateFormula(options);
            Console.WriteLine($"First calculation - Changed: {monitor.Changed}");

            // Ändra värde och beräkna om
            worksheet.Cells["A1"].Value = 20;
            monitor.Changed = false;
            workbook.CalculateFormula(options);
            Console.WriteLine($"Second calculation - Changed: {monitor.Changed}");
        }
    }
}
```

### Se även

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


