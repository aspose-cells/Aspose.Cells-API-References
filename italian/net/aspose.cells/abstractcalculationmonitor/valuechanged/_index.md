---
title: "AbstractCalculationMonitor.ValueChanged"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AbstractCalculationMonitor. Indica se il valore della cella è stato modificato dopo il calcolo. Deve essere usata solo in AfterCalculate"
type: docs
url: /it/net/aspose.cells/abstractcalculationmonitor/valuechanged/
---
## AbstractCalculationMonitor.ValueChanged property

Indica se il valore della cella è stato modificato dopo il calcolo. Deve essere usata solo in [`AfterCalculate`](../aftercalculate/).

```csharp
public bool ValueChanged { get; }
```

### Esempi

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

            // Imposta il valore iniziale
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Formula = "=A1*2";

            // Crea e imposta il monitor di calcolo
            CustomCalculationMonitor2 monitor = new CustomCalculationMonitor2();
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = monitor;

            // Primo calcolo
            workbook.CalculateFormula(options);
            Console.WriteLine($"First calculation - Changed: {monitor.Changed}");

            // Modifica valore e ricalcola
            worksheet.Cells["A1"].Value = 20;
            monitor.Changed = false;
            workbook.CalculateFormula(options);
            Console.WriteLine($"Second calculation - Changed: {monitor.Changed}");
        }
    }
}
```

### Vedi anche

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


