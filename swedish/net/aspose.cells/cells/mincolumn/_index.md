---
title: "Cells.MinColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Minsta kolumnindex för de celler som har instansierats i samlingen, inkluderar inte den kolumn där stil är definierad för hela kolumnen men ingen cell har instansierats i den."
type: docs
url: /sv/net/aspose.cells/cells/mincolumn/
---
## Cells.MinColumn property

Minsta kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den).

```csharp
public int MinColumn { get; }
```

### Anmärkningar

Denna egenskap måste iterera och kontrollera celler och rader dynamiskt, så det är en tidskrävande process och bör inte anropas upprepade gånger, till exempel genom att använda den direkt som villkor i en loop.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till cells-samlingen
            Cells cells = worksheet.Cells;
            
            // Fyll i lite data i kolumnerna 2, 3 och 4 (B, C, D)
            cells["B1"].PutValue("Data in Column B");
            cells["C1"].PutValue("Data in Column C");
            cells["D1"].PutValue("Data in Column D");
            
            // Hämta det minsta kolumnindexet som innehåller data
            int minColumn = cells.MinColumn;
            
            // Hämta det största kolumnindexet som innehåller data
            int maxColumn = cells.MaxColumn;
            
            Console.WriteLine("Minimum column with data: " + minColumn); // Should output 1 (column B)
            Console.WriteLine("Maximum column with data: " + maxColumn); // Should output 3 (column D)
            
            // Rensa kolumn B för att demonstrera MinColumn-ändring
            cells.DeleteColumn(1);
            
            Console.WriteLine("\nAfter deleting column B:");
            Console.WriteLine("New minimum column with data: " + cells.MinColumn); // Should now output 2 (column C)
            Console.WriteLine("Maximum column with data: " + cells.MaxColumn); // Should still output 3 (column D)
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


