---
title: "AbstractCalculationMonitor.CalculatedValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractCalculationMonitor-egenskap. Hämtar det nyberäknade värdet för cellen. Bör endast användas i AfterCalculate"
type: docs
url: /sv/net/aspose.cells/abstractcalculationmonitor/calculatedvalue/
---
## AbstractCalculationMonitor.CalculatedValue property

Hämtar det nyberäknade värdet för cellen. Bör endast användas i [`AfterCalculate`](../aftercalculate/).

```csharp
public object CalculatedValue { get; }
```

### Exempel

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

            // Ställ in beräkningskedjan
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";

            // Skapa och anslut monitor
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = monitor;

            // Utlösa beräkning som kommer att anropa vår monitor
            workbook.CalculateFormula(options);

            // Ändra ett värde för att utlösa notifiering om värdeförändring
            worksheet.Cells["A1"].Value = 5;
            workbook.CalculateFormula(options);
        }
    }
}
```

### Se även

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


