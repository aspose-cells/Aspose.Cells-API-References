---
title: "AbstractCalculationMonitor.CalculatedValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AbstractCalculationMonitor. Restituisce il valore appena calcolato della cella. Deve essere usata solo in AfterCalculate"
type: docs
url: /it/net/aspose.cells/abstractcalculationmonitor/calculatedvalue/
---
## AbstractCalculationMonitor.CalculatedValue property

Restituisce il valore appena calcolato della cella. Deve essere usata solo in [`AfterCalculate`](../aftercalculate/).

```csharp
public object CalculatedValue { get; }
```

### Esempi

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

            // Configura la catena di calcolo
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";

            // Crea e collega il monitor
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = monitor;

            // Avvia il calcolo che invocherà il nostro monitor
            workbook.CalculateFormula(options);

            // Modifica un valore per attivare la notifica di cambiamento del valore
            worksheet.Cells["A1"].Value = 5;
            workbook.CalculateFormula(options);
        }
    }
}
```

### Vedi anche

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


