---
title: "CellWatchCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellWatchCollection-metoden. Lägger till CellWatch med en rad och en kolumn"
type: docs
url: /sv/net/aspose.cells/cellwatchcollection/add/
---
## Add(int, int) {#add}

Lägger till [`CellWatch`](../../cellwatch/) med en rad och en kolumn.

```csharp
public int Add(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |
| column | Int32 | Kolumnindexet. |

### Returvärde

Returnerar positionen för detta objekt i samlingen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta CellWatchCollection från kalkylbladet
            CellWatchCollection cellWatchCollection = worksheet.CellWatches;
            
            try
            {
                // Anropa Add-metoden med rad- och kolumnindex (Int32, Int32)
                int index = cellWatchCollection.Add(5, 3); // Adding cell at row 6, column D (0-based)
                
                Console.WriteLine($"CellWatch added at index: {index}");
                
                // Verifiera den tillagda CellWatch
                CellWatch cellWatch = cellWatchCollection[index];
                Console.WriteLine($"Watching cell: {cellWatch.Row},{cellWatch.Column}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("CellWatchCollectionMethodAddWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Lägger till [`CellWatch`](../../cellwatch/) med namnet på cellen.

```csharp
public int Add(string cellName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Namnet på cellen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till några cellövervakningar
            worksheet.CellWatches.Add("A1");
            worksheet.CellWatches.Add("B2");
            worksheet.CellWatches.Add("C3");
            
            // Visa antalet cell watches
            Console.WriteLine("Cell Watches Count: " + worksheet.CellWatches.Count);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


