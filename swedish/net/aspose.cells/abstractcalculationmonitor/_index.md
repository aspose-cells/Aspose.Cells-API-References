---
title: "Klass AbstractCalculationMonitor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.AbstractCalculationMonitor-klass. Övervakar för användaren att följa framstegen i formelberäkningen"
type: docs
url: /sv/net/aspose.cells/abstractcalculationmonitor/
---
## AbstractCalculationMonitor class

Övervaka för att användaren ska kunna följa framstegen i formelberäkningen.

```csharp
public abstract class AbstractCalculationMonitor
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CalculatedValue](../../aspose.cells/abstractcalculationmonitor/calculatedvalue/) { get; } | Hämtar det nyberäknade värdet för cellen. Ska endast användas i [`AfterCalculate`](./aftercalculate/). |
| [OriginalValue](../../aspose.cells/abstractcalculationmonitor/originalvalue/) { get; } | Hämtar det gamla värdet för den beräknade cellen. Ska endast användas i [`BeforeCalculate`](./beforecalculate/) och [`AfterCalculate`](./aftercalculate/). |
| [ValueChanged](../../aspose.cells/abstractcalculationmonitor/valuechanged/) { get; } | Om cellens värde har ändrats efter beräkningen. Ska endast användas i [`AfterCalculate`](./aftercalculate/). |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [AfterCalculate](../../aspose.cells/abstractcalculationmonitor/aftercalculate/)(int, int, int) | Implementera den här metoden för att utföra affärslogik efter att en cell har beräknats. |
| virtual [BeforeCalculate](../../aspose.cells/abstractcalculationmonitor/beforecalculate/)(int, int, int) | Implementera den här metoden för att utföra affärslogik innan en cell beräknas. |
| virtual [OnCircular](../../aspose.cells/abstractcalculationmonitor/oncircular/)(IEnumerator) | Implementera den här metoden för att utföra affärslogik när du beräknar formler med cirkulära referenser. |

### Exempel

```csharp
using Aspose.Cells;
using System;
using System.Collections;

namespace AsposeCellsExamples
{
    // Anpassad implementation av AbstractCalculationMonitor
    public class CustomCalculationMonitor : AbstractCalculationMonitor
    {
        public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"Before calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"After calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
            Console.WriteLine($"Original Value: {OriginalValue}, Calculated Value: {CalculatedValue}, Value Changed: {ValueChanged}");
        }

        public override bool OnCircular(IEnumerator circularCellsData)
        {
            Console.WriteLine("Circular reference detected.");
            return false; // Return false to stop calculation when circular reference is detected
        }
    }

    public class CalculationMonitorDemo
    {
        public static void RunDemo()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // Skapa en instans av CustomCalculationMonitor
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();

            // Ställ in beräkningsalternativ
            CalculationOptions options = new CalculationOptions
            {
                CalculationMonitor = monitor,
                IgnoreError = false,
                Recursive = true
            };

            // Beräkna formler med den anpassade monitorn
            workbook.CalculateFormula(options);

            // Spara arbetsboken
            workbook.Save("CalculationMonitorDemo.xlsx");
            workbook.Save("CalculationMonitorDemo.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


