---
title: "CellWatchCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellWatchCollection. Ottiene e imposta CellWatch per indice"
type: docs
url: /it/net/aspose.cells/cellwatchcollection/item/
---
## CellWatchCollection indexer (1 of 2)

Ottiene e imposta [`CellWatch`](../../cellwatch/) per indice.

```csharp
public CellWatch this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatchCollection cellWatches = sheet.CellWatches;
            
            // Dimostra l'uso della proprietà Item
            CellWatch cellWatch = cellWatches[watchIndex];
            
            Console.WriteLine("Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            cellWatch.Row = 1;
            cellWatch.Column = 1;
            cellWatch.CellName = "A1";
            
            Console.WriteLine("\nModified Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            workbook.Save("CellWatchCollectionExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CellWatchCollection indexer (2 of 2)

Ottiene e imposta [`CellWatch`](../../cellwatch/) per il nome della cella.

```csharp
public CellWatch this[string cellName] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| cellName | Il nome della cella. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Ottieni il primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi un monitor della cella alla raccolta
                int watchIndex = worksheet.CellWatches.Add("A1");

                // Accedi alla CellWatchCollection
                CellWatchCollection cellWatches = worksheet.CellWatches;

                // Dimostra l'accesso alla proprietà Item usando l'indicizzatore
                CellWatch cellWatch = cellWatches[watchIndex];

                // Visualizza le proprietà dell'elemento CellWatch
                Console.WriteLine("Cell Watch Details:");
                Console.WriteLine($"Row: {cellWatch.Row}");
                Console.WriteLine($"Column: {cellWatch.Column}");
                Console.WriteLine($"Cell Name: {cellWatch.CellName}");

                // Salva la cartella di lavoro
                workbook.Save("CellWatchItemDemo.xlsx");
                Console.WriteLine("Item property has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


