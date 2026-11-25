---
title: "Cell.IsErrorValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Verifica se il valore di questa cella è un errore"
type: docs
url: /it/net/aspose.cells/cell/iserrorvalue/
---
## Cell.IsErrorValue property

Verifica se il valore di questa cella è un errore.

```csharp
public bool IsErrorValue { get; }
```

### Osservazioni

Vale anche per le celle formula per verificare se il risultato calcolato è un errore.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsErrorValueDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta una formula che produrrà un errore
            Cell cell = cells["A1"];
            cell.Formula = "=1/0"; // Division by zero error
            
            // Calcola le formule
            workbook.CalculateFormula();

            // Dimostra la proprietà IsErrorValue
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("IsErrorValue: " + cell.IsErrorValue);
            Console.WriteLine("Error type: " + cell.Value);

            // Imposta un valore valido
            Cell cell2 = cells["A2"];
            cell2.PutValue("Valid value");
            
            Console.WriteLine("\nCell A2 value: " + cell2.StringValue);
            Console.WriteLine("IsErrorValue: " + cell2.IsErrorValue);

            // Imposta un errore SPILL (errore di formula di array dinamico di Excel 365+)
            Cell cell3 = cells["A3"];
            cell3.SetDynamicArrayFormula("=A1:A10", new FormulaParseOptions(), true);
            
            Console.WriteLine("\nCell A3 value: " + cell3.StringValue);
            Console.WriteLine("IsErrorValue: " + cell3.IsErrorValue);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


