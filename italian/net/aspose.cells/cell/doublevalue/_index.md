---
title: "Cell.DoubleValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Restituisce il valore double contenuto nella cella"
type: docs
url: /it/net/aspose.cells/cell/doublevalue/
---
## Cell.DoubleValue property

Restituisce il valore double contenuto nella cella.

```csharp
public double DoubleValue { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDoubleValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta diversi tipi di valore nelle celle
            cells["A1"].PutValue(1); // Int value
            cells["A2"].PutValue(true); // Bool value
            cells["A3"].PutValue("abc"); // String value
            cells["A4"].PutValue(false); // Bool value
            cells["A5"].PutValue(2.56); // Double value

            // Dimostra la proprietà DoubleValue
            Console.WriteLine("Double value from cell A5: " + cells["A5"].DoubleValue);
            
            // Verifica che altri tipi di valore possano essere letti come double
            Console.WriteLine("Int as double from A1: " + cells["A1"].DoubleValue);
            Console.WriteLine("Bool as double from A2: " + cells["A2"].DoubleValue);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


