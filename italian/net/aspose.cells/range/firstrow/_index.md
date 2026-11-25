---
title: "Range.FirstRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Restituisce l'indice della prima riga dell'intervallo"
type: docs
url: /it/net/aspose.cells/range/firstrow/
---
## Range.FirstRow property

Ottiene l'indice della prima riga dell'intervallo.

```csharp
public int FirstRow { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstRowDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Crea un intervallo
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Accedi e visualizza la proprietà FirstRow
            Console.WriteLine("First row index of range: " + range.FirstRow);

            // Accedi alla prima cella nella prima riga dell'intervallo
            Cell firstCell = worksheet.Cells[range.FirstRow, range.FirstColumn];
            Console.WriteLine("First cell value: " + firstCell.StringValue);
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


