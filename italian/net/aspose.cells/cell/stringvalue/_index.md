---
title: "Cell.StringValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Ottiene il valore stringa contenuto nella cella. Se il tipo di questa cella è stringa, restituisce il valore stringa stesso. Per gli altri tipi di cella, verrà restituito il valore stringa formattato con lo stile specificato per questa cella. Il valore della cella formattato è lo stesso di quello che si ottiene da Excel copiando una cella come testo, ad esempio copiando la cella in un editor di testo o esportando in CSV."
type: docs
url: /it/net/aspose.cells/cell/stringvalue/
---
## Cell.StringValue property

Ottiene il valore stringa contenuto nella cella. Se il tipo di questa cella è stringa, restituisce il valore stringa stesso. Per gli altri tipi di cella, verrà restituito il valore stringa formattato (formattato con lo stile specificato di questa cella). Il valore della cella formattato è lo stesso di quello che si ottiene da Excel copiando una cella come testo (ad esempio copiando la cella in un editor di testo o esportando in CSV).

```csharp
public string StringValue { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyStringValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta alcuni valori
            cells["A1"].PutValue("Hello");
            cells["A2"].PutValue(123);
            cells["A3"].PutValue(DateTime.Now);
            cells["A4"].Formula = "=A1&A2";

            // Calcola le formule
            workbook.CalculateFormula();

            // Dimostra la proprietà StringValue
            Console.WriteLine("A1 StringValue: " + cells["A1"].StringValue);
            Console.WriteLine("A2 StringValue: " + cells["A2"].StringValue);
            Console.WriteLine("A3 StringValue: " + cells["A3"].StringValue);
            Console.WriteLine("A4 StringValue: " + cells["A4"].StringValue);

            // Mostra il caso di valore di errore
            Cell errorCell = cells["B1"];
            errorCell.Formula = "=1/0";
            workbook.CalculateFormula();
            Console.WriteLine("B1 (Error) StringValue: " + errorCell.StringValue);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


