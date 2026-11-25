---
title: "FindOptions.IsRangeSet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FindOptions. Indica se l'intervallo di ricerca è impostato"
type: docs
url: /it/net/aspose.cells/findoptions/israngeset/
---
## FindOptions.IsRangeSet property

Indica se l'intervallo cercato è impostato.

```csharp
public bool IsRangeSet { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertyIsRangeSetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Date");
            worksheet.Cells["B2"].PutValue("Elderberry");
            worksheet.Cells["B3"].PutValue("Fig");

            // Crea un'istanza di FindOptions
            FindOptions findOptions = new FindOptions();

            // Verifica il valore iniziale di IsRangeSet (dovrebbe essere false)
            Console.WriteLine("Initial IsRangeSet value: " + findOptions.IsRangeSet);

            // Imposta un intervallo di ricerca
            CellArea searchRange = new CellArea();
            searchRange.StartRow = 0;
            searchRange.StartColumn = 0;
            searchRange.EndRow = 2;
            searchRange.EndColumn = 0; // Column A only
            findOptions.SetRange(searchRange);

            // Verifica IsRangeSet dopo aver impostato l'intervallo (dovrebbe essere true)
            Console.WriteLine("After SetRange, IsRangeSet value: " + findOptions.IsRangeSet);

            // Esegui un'operazione di ricerca all'interno dell'intervallo specificato
            Cell foundCell = worksheet.Cells.Find("Banana", null, findOptions);
            Console.WriteLine("Found 'Banana' at: " + foundCell?.Name);

            // Prova a trovare qualcosa al di fuori dell'intervallo (non dovrebbe essere trovato)
            foundCell = worksheet.Cells.Find("Fig", null, findOptions);
            Console.WriteLine("Found 'Fig' at: " + foundCell?.Name); // Should be null

            // Salva la cartella di lavoro
            workbook.Save("PropertyIsRangeSetDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


