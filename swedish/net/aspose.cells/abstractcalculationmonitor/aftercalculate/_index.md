---
title: "AbstractCalculationMonitor.AfterCalculate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractCalculationMonitor-metod. Implementera denna metod för att utföra affärslogik efter att en cell har beräknats"
type: docs
url: /sv/net/aspose.cells/abstractcalculationmonitor/aftercalculate/
---
## AbstractCalculationMonitor.AfterCalculate method

Implementera den här metoden för att utföra affärslogik efter att en cell har beräknats.

```csharp
public virtual void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | Int32 | Index för bladet som cellen tillhör. |
| rowIndex | Int32 | Radindex för cellen |
| colIndex | Int32 | Kolumnindex för cellen |

### Exempel

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

            // Skapa exempelformler
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

### Se även

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


