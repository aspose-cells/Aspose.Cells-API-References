---
title: "Row.Index"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Row proprietà. Ottiene l'indice di questa riga"
type: docs
url: /it/net/aspose.cells/row/index/
---
## Row.Index property

Ottiene l'indice di questa riga.

```csharp
public int Index { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIndexDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati alle celle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Itera attraverso le righe e dimostra la proprietà Index
            foreach (Row row in worksheet.Cells.Rows)
            {
                Console.WriteLine($"Processing row with index: {row.Index}");
                if (row.Index > 0) // Skip header row
                {
                    Console.WriteLine($"Data in row {row.Index}: " +
                        $"{worksheet.Cells[row.Index, 0].StringValue}, " +
                        $"{worksheet.Cells[row.Index, 1].IntValue}");
                }
            }
        }
    }
}
```

### Vedi anche

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


