---
title: "Cell.IsNumericValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Cell proprietà. Indica se il valore di questa cella è numerico, intero, double e datetime"
type: docs
url: /it/net/aspose.cells/cell/isnumericvalue/
---
## Cell.IsNumericValue property

Indica se il valore di questa cella è numerico (int, double e datetime).

```csharp
public bool IsNumericValue { get; }
```

### Osservazioni

Si applica anche alle celle di formula per verificare il risultato calcolato

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsNumericValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi diversi tipi di dati alle celle
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue(123.45); // Numeric value

            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Hello World"); // String value

            // Verifica se le celle contengono valori numerici
            Console.WriteLine("Cell A1 IsNumericValue: " + cell1.IsNumericValue);
            Console.WriteLine("Cell A2 IsNumericValue: " + cell2.IsNumericValue);

            // Dimostra l'uso con logica condizionale
            if (cell1.IsNumericValue)
            {
                Console.WriteLine("Cell A1 contains a numeric value: " + cell1.DoubleValue);
            }

            if (!cell2.IsNumericValue)
            {
                Console.WriteLine("Cell A2 does not contain a numeric value");
            }
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


