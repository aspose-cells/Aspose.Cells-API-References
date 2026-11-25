---
title: "CellRichValue.ErrorValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellRichValue. Ottiene il tipo di valore di errore della cella"
type: docs
url: /it/net/aspose.cells/cellrichvalue/errorvalue/
---
## CellRichValue.ErrorValue property

Ottiene il tipo di valore di errore della cella.

```csharp
public virtual ErrorCellValueType ErrorValue { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellRichValuePropertyErrorValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un errore di spill nella cella A1
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3})";
            
            try
            {
                // Calcola le formule per generare l'errore di spill
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // Errore spill previsto.
            }
            
            // Ottieni il valore ricco dalla cella A1
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // Verifica e visualizza il tipo di errore
            Console.WriteLine("Error type: " + richValue.ErrorValue);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ErrorCellValueType](../../errorcellvaluetype/)
* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


