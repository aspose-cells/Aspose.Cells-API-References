---
title: "Cells.GetEnumerator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar cellernas enumerator"
type: docs
url: /sv/net/aspose.cells/cells/getenumerator/
---
## Cells.GetEnumerator method

Hämtar cellernas enumerator.

```csharp
public IEnumerator GetEnumerator()
```

### Returvärde

Cellernas enumerator

### Anmärkningar

När du traverserar element med den returnerade Enumeratorn bör cellsamlingen inte modifieras (såsom operationer som skapar nya Cell/Row eller tar bort befintliga Cell/Row). Annars kan enumeratorn misslyckas med att traversera alla celler korrekt (vissa element kan traverseras flera gånger eller hoppas över).

### Exempel

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            
            // Hämta enumerator och iterera genom celler
            IEnumerator enumerator = worksheet.Cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                if (cell.Value != null)
                {
                    Console.WriteLine($"{cell.Name}: {cell.Value}");
                }
            }
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


