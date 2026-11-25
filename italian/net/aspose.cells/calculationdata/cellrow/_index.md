---
title: "CalculationData.CellRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationData. Ottiene l'indice di riga della cella in cui si trova la funzione"
type: docs
url: /it/net/aspose.cells/calculationdata/cellrow/
---
## CalculationData.CellRow property

Ottiene l'indice della riga della cella in cui si trova la funzione.

```csharp
public int CellRow { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCellRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta alcuni dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Imposta le opzioni di calcolo
            CalculationOptions opts = new CalculationOptions();
            opts.CustomEngine = new CustomCalculationEngine();

            // Calcola le formule
            workbook.CalculateFormula(opts);

            // Accedi alla cella calcolata e dimostra la proprietà CellRow
            Cell calculatedCell = worksheet.Cells["A3"];
            Console.WriteLine("Calculated cell is at row: " + calculatedCell.Row);
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Dimostrare l'accesso alle informazioni di riga dai dati di calcolo
            if (data != null)
            {
                Console.WriteLine("Current calculation is for row: " + data.CellRow);
            }
        }
    }
}
```

### Vedi anche

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


