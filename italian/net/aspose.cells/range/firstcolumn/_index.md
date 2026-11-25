---
title: "Range.FirstColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Ottiene l'indice della prima colonna dell'intervallo"
type: docs
url: /it/net/aspose.cells/range/firstcolumn/
---
## Range.FirstColumn property

Ottiene l'indice della prima colonna dell'intervallo.

```csharp
public int FirstColumn { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // Crea un intervallo
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");

            // Dimostra la proprietà FirstColumn
            Console.WriteLine("First column index of range: " + range.FirstColumn);

            // Usa FirstColumn per accedere alle celle nella prima colonna dell'intervallo
            for (int i = 0; i < range.RowCount; i++)
            {
                Cell cell = range[i, 0]; // Access first column (index 0) of the range
                Console.WriteLine($"Cell[{i},0] value: {cell.StringValue}");
            }

            // Salva la cartella di lavoro
            workbook.Save("RangeFirstColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


