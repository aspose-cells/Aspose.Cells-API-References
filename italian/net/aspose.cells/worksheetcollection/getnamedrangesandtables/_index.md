---
title: "WorksheetCollection.GetNamedRangesAndTables"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorksheetCollection. Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo"
type: docs
url: /it/net/aspose.cells/worksheetcollection/getnamedrangesandtables/
---
## WorksheetCollection.GetNamedRangesAndTables method

Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo.

```csharp
public Range[] GetNamedRangesAndTables()
```

### Valore di ritorno

Un array di oggetti Range.

Restituisce null se l'intervallo denominato non esiste.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetNamedRangesAndTablesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea alcuni intervalli denominati
            worksheet.Cells.CreateRange("A1:B2").Name = "TestRange1";
            worksheet.Cells.CreateRange("C3:D4").Name = "TestRange2";
            
            // Ottieni tutti gli intervalli denominati e le tabelle
            Aspose.Cells.Range[] ranges = workbook.Worksheets.GetNamedRangesAndTables();
            
            // Visualizza le informazioni sugli intervalli
            Console.WriteLine("Found {0} named ranges:", ranges.Length);
            foreach (Aspose.Cells.Range range in ranges)
            {
                Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
            }
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


