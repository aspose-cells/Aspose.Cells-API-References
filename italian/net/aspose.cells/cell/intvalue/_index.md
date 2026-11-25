---
title: "Cell.IntValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Restituisce il valore intero contenuto nella cella"
type: docs
url: /it/net/aspose.cells/cell/intvalue/
---
## Cell.IntValue property

Restituisce il valore intero contenuto nella cella.

```csharp
public int IntValue { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIntValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Imposta un valore numerico e ottieni IntValue
            Cell cell1 = cells[0, 0];
            cell1.PutValue(42);
            Console.WriteLine("IntValue of numeric cell: " + cell1.IntValue);

            // Imposta una formula che restituisce un numero e ottieni IntValue
            Cell cell2 = cells[0, 1];
            cell2.Formula = "=10+5";
            workbook.CalculateFormula();
            Console.WriteLine("IntValue of formula cell: " + cell2.IntValue);

            // Imposta un valore booleano e ottieni IntValue
            Cell cell3 = cells[0, 2];
            cell3.PutValue(true);
            Console.WriteLine("IntValue of boolean cell: " + cell3.IntValue);

            // Imposta un valore di testo e ottieni IntValue (sarà 0 se non convertibile)
            Cell cell4 = cells[0, 3];
            cell4.PutValue("Hello");
            Console.WriteLine("IntValue of text cell: " + cell4.IntValue);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


