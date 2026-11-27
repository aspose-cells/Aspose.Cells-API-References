---
title: "CellWatchCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellWatchCollection-egenskapen. Hämtar och anger CellWatch efter index"
type: docs
url: /sv/net/aspose.cells/cellwatchcollection/item/
---
## CellWatchCollection indexer (1 of 2)

Hämtar och anger [`CellWatch`](../../cellwatch/) efter index.

```csharp
public CellWatch this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Exempel

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
            
            // Demonstrera användning av Item-egenskapen
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

### Se även

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CellWatchCollection indexer (2 of 2)

Hämtar och anger [`CellWatch`](../../cellwatch/) efter cellens namn.

```csharp
public CellWatch this[string cellName] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| cellName | Namnet på cellen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Hämta det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till en cellövervakning i samlingen
                int watchIndex = worksheet.CellWatches.Add("A1");

                // Åtkomst till CellWatchCollection
                CellWatchCollection cellWatches = worksheet.CellWatches;

                // Visa hur man får åtkomst till Item-egenskapen med indexerare
                CellWatch cellWatch = cellWatches[watchIndex];

                // Visa egenskaperna för CellWatch-objektet
                Console.WriteLine("Cell Watch Details:");
                Console.WriteLine($"Row: {cellWatch.Row}");
                Console.WriteLine($"Column: {cellWatch.Column}");
                Console.WriteLine($"Cell Name: {cellWatch.CellName}");

                // Spara arbetsboken
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

### Se även

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


