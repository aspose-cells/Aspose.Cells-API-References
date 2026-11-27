---
title: "Range.GetEnumerator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Hämtar enumeratorn för celler i detta Range"
type: docs
url: /sv/net/aspose.cells/range/getenumerator/
---
## Range.GetEnumerator method

Hämtar enumeratorn för celler i detta område.

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
    public class RangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i lite exempeldata
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Banana");
            worksheet.Cells["C2"].PutValue("Cherry");
            worksheet.Cells["C3"].PutValue("Date");

            // Hämta range och iterera genom celler
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C3");
            IEnumerator enumerator = range.GetEnumerator();
            
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine($"{cell.Name}: {cell.Value}");
            }
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


