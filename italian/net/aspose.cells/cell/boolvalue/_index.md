---
title: "Cell.BoolValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Ottiene il valore booleano contenuto nella cella"
type: docs
url: /it/net/aspose.cells/cell/boolvalue/
---
## Cell.BoolValue property

Restituisce il valore booleano contenuto nella cella.

```csharp
public bool BoolValue { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyBoolValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            
            // Imposta una formula che restituisce un valore booleano
            cell.Formula = "=2.01>2";
            
            // Calcola la formula per ottenere il risultato
            workbook.CalculateFormula();
            
            // Dimostra la proprietà BoolValue
            Console.WriteLine("Cell BoolValue: " + cell.BoolValue);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


