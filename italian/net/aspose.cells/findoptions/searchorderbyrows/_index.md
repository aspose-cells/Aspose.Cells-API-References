---
title: "FindOptions.SearchOrderByRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FindOptions. Indica se l'ordine di ricerca è per righe o colonne"
type: docs
url: /it/net/aspose.cells/findoptions/searchorderbyrows/
---
## FindOptions.SearchOrderByRows property

Indica se l'ordine di ricerca è per righe o colonne.

```csharp
public bool SearchOrderByRows { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertySearchOrderByRowsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e aggiungi dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola le celle con dati di test (cerca "abc" in ordine colonna-prima)
            worksheet.Cells["A1"].PutValue("xyz");
            worksheet.Cells["B1"].PutValue("def");
            worksheet.Cells["A2"].PutValue("123");
            worksheet.Cells["B2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("abc");
            worksheet.Cells["B3"].PutValue("789");

            // Crea le opzioni di ricerca e imposta l'ordine di ricerca su colonna-prima
            FindOptions findOptions = new FindOptions();
            findOptions.SearchOrderByRows = false; // Search column by column

            // Trova "abc" - dovrebbe restituire A3 (riga 2, colonna 0) quando si ricerca in ordine colonna-prima
            Cell foundCell = worksheet.Cells.Find("abc", null, findOptions);

            // Restituisci il risultato
            Console.WriteLine($"Found 'abc' at row: {foundCell.Row}, column: {foundCell.Column}");
        }
    }
}
```

### Vedi anche

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


