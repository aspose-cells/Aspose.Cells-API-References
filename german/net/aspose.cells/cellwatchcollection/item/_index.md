---
title: "CellWatchCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellWatchCollection-Eigenschaft. Ruft CellWatch nach Index ab und legt sie fest"
type: docs
url: /de/net/aspose.cells/cellwatchcollection/item/
---
## CellWatchCollection indexer (1 of 2)

Ruft [`CellWatch`](../../cellwatch/) nach Index ab und legt sie fest.

```csharp
public CellWatch this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Beispiele

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
            
            // Demonstriere die Verwendung der Item-Eigenschaft
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

### Siehe auch

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CellWatchCollection indexer (2 of 2)

Ruft [`CellWatch`](../../cellwatch/) nach dem Namen der Zelle ab und legt sie fest.

```csharp
public CellWatch this[string cellName] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| cellName | Der Name der Zelle. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Hole das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Füge eine cell watch zur Sammlung hinzu
                int watchIndex = worksheet.CellWatches.Add("A1");

                // Greife auf die CellWatchCollection zu.
                CellWatchCollection cellWatches = worksheet.CellWatches;

                // Demonstrieren Sie den Zugriff auf die Item-Eigenschaft mittels Indexer
                CellWatch cellWatch = cellWatches[watchIndex];

                // Zeige die Eigenschaften des CellWatch‑Elements an.
                Console.WriteLine("Cell Watch Details:");
                Console.WriteLine($"Row: {cellWatch.Row}");
                Console.WriteLine($"Column: {cellWatch.Column}");
                Console.WriteLine($"Cell Name: {cellWatch.CellName}");

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


