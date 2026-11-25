---
title: "AbstractCalculationMonitor.OriginalValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AbstractCalculationMonitor. Restituisce il valore precedente della cella calcolata. Deve essere usata solo in BeforeCalculate e AfterCalculate"
type: docs
url: /it/net/aspose.cells/abstractcalculationmonitor/originalvalue/
---
## AbstractCalculationMonitor.OriginalValue property

Restituisce il valore precedente della cella calcolata. Deve essere usata solo in [`BeforeCalculate`](../beforecalculate/) e [`AfterCalculate`](../aftercalculate/).

```csharp
public object OriginalValue { get; }
```

### Esempi

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

            // Imposta il valore iniziale
            worksheet.Cells["A1"].PutValue(10);
            
            // Aggiungi una formula che cambierà il valore
            worksheet.Cells["A2"].Formula = "=A1*2";
            
            // Imposta il monitor di calcolo
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CustomCalculationMonitor1();
            
            // Ricalcola le formule - questo attiverà il monitor
            workbook.CalculateFormula(options);
            
            // Modifica il valore originale per dimostrare il monitor
            worksheet.Cells["A1"].PutValue(20);
            workbook.CalculateFormula(options);
        }
    }
}
```

### Vedi anche

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


