---
title: "AbstractCalculationMonitor.AfterCalculate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractCalculationMonitor. Implementa questo metodo per eseguire operazioni dopo che una cella è stata calcolata"
type: docs
url: /it/net/aspose.cells/abstractcalculationmonitor/aftercalculate/
---
## AbstractCalculationMonitor.AfterCalculate method

Implementa questo metodo per eseguire operazioni dopo che una cella è stata calcolata.

```csharp
public virtual void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | Int32 | Indice del foglio a cui appartiene la cella. |
| rowIndex | Int32 | Indice di riga della cella |
| colIndex | Int32 | Indice di colonna della cella |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationMonitorMethodAfterCalculateWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Configura le formule di esempio
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["B1"].Formula = "=NOW()"; // Volatile function

            CalculationOptions options = new CalculationOptions();
            var monitor = new CalculationMonitor();
            options.CalculationMonitor = monitor;

            try
            {
                workbook.CalculateFormula(options);
                Console.WriteLine("Calculation completed. Check cell values and console output.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("AfterCalculateDemo.xlsx");
        }


        private class CalculationMonitor : AbstractCalculationMonitor
        {
            public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
            {
                Console.WriteLine($"Calculated cell (Sheet {sheetIndex}): Row {rowIndex}, Column {colIndex}");
                Console.WriteLine($"Value changed: {ValueChanged}, Original: {OriginalValue}, New: {CalculatedValue}");
                Console.WriteLine("----------------------------------");
            }
        }
    }
}
```

### Vedi anche

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


