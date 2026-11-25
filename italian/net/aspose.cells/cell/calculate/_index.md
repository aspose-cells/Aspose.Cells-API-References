---
title: "Cell.Calculate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Calcola la formula della cella"
type: docs
url: /it/net/aspose.cells/cell/calculate/
---
## Cell.Calculate method

Calcola la formula della cella.

```csharp
public void Calculate(CalculationOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | CalculationOptions | Opzioni per il calcolo |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodCalculateWithCalculationOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta una formula semplice nella cella A1
            Cell cellA1 = worksheet.Cells["A1"];
            cellA1.Formula = "=SUM(1, 2, 3)";
            
            // Calcola con le opzioni predefinite
            cellA1.Calculate(new CalculationOptions());
            Console.WriteLine("A1 value after calculation: " + cellA1.Value);

            // Imposta una formula matriciale nell'intervallo B1:D1
            Cell cellB1 = worksheet.Cells["B1"];
            cellB1.SetArrayFormula("={1,2,3}", 1, 3);
            
            // Calcola la formula matriciale con opzioni
            cellB1.Calculate(new CalculationOptions());
            Console.WriteLine("B1 value after calculation: " + cellB1.Value);

            // Imposta una formula più complessa nella cella A2
            Cell cellA2 = worksheet.Cells["A2"];
            cellA2.Formula = "=IF(A1>5, \"Greater\", \"Less or equal\")";
            
            // Calcola con opzioni
            cellA2.Calculate(new CalculationOptions());
            Console.WriteLine("A2 value after calculation: " + cellA2.Value);
        }
    }
}
```

### Vedi anche

* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


