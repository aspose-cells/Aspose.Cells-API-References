---
title: "Classe AbstractCalculationMonitor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.AbstractCalculationMonitor. Monitor per l'utente per tenere traccia dell'avanzamento del calcolo delle formule"
type: docs
url: /it/net/aspose.cells/abstractcalculationmonitor/
---
## AbstractCalculationMonitor class

Monitor per l'utente per tenere traccia dell'avanzamento del calcolo della formula.

```csharp
public abstract class AbstractCalculationMonitor
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CalculatedValue](../../aspose.cells/abstractcalculationmonitor/calculatedvalue/) { get; } | Ottiene il valore appena calcolato della cella. Deve essere usato solo in [`AfterCalculate`](./aftercalculate/). |
| [OriginalValue](../../aspose.cells/abstractcalculationmonitor/originalvalue/) { get; } | Ottiene il valore precedente della cella calcolata. Deve essere usato solo in [`BeforeCalculate`](./beforecalculate/) e [`AfterCalculate`](./aftercalculate/). |
| [ValueChanged](../../aspose.cells/abstractcalculationmonitor/valuechanged/) { get; } | Indica se il valore della cella è stato modificato dopo il calcolo. Deve essere usato solo in [`AfterCalculate`](./aftercalculate/). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [AfterCalculate](../../aspose.cells/abstractcalculationmonitor/aftercalculate/)(int, int, int) | Implementa questo metodo per eseguire operazioni dopo che una cella è stata calcolata. |
| virtual [BeforeCalculate](../../aspose.cells/abstractcalculationmonitor/beforecalculate/)(int, int, int) | Implementa questo metodo per eseguire operazioni prima di calcolare una cella. |
| virtual [OnCircular](../../aspose.cells/abstractcalculationmonitor/oncircular/)(IEnumerator) | Implementa questo metodo per gestire la logica di business durante il calcolo delle formule con riferimenti circolari. |

### Esempi

```csharp
using Aspose.Cells;
using System;
using System.Collections;

namespace AsposeCellsExamples
{
    // Implementazione personalizzata di AbstractCalculationMonitor
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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // Crea un'istanza di CustomCalculationMonitor
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();

            // Imposta le opzioni di calcolo
            CalculationOptions options = new CalculationOptions
            {
                CalculationMonitor = monitor,
                IgnoreError = false,
                Recursive = true
            };

            // Calcola le formule con il monitor personalizzato
            workbook.CalculateFormula(options);

            // Salva la cartella di lavoro
            workbook.Save("CalculationMonitorDemo.xlsx");
            workbook.Save("CalculationMonitorDemo.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


