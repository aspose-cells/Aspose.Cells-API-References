---
title: "Cell.Formula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Ottiene o imposta una formula della Cell."
type: docs
url: /it/net/aspose.cells/cell/formula/
---
## Cell.Formula property

Ottiene o imposta una formula del [`Cell`](../).

```csharp
public string Formula { get; set; }
```

### Osservazioni

Una stringa di formula inizia sempre con un segno uguale (=). E per favore usa sempre la virgola (,) come delimitatore dei parametri, ad esempio "=SUM(A1, E1, H2)".

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta i valori nelle celle che saranno usati nella formula
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["E1"].PutValue(5);
            worksheet.Cells["A1"].PutValue(100);

            // Imposta la formula nella cella B6
            worksheet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + A1";

            // Calcola la formula
            workbook.CalculateFormula();

            // Visualizza il risultato
            Console.WriteLine("Formula result in B6: " + worksheet.Cells["B6"].Value);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


