---
title: "RangeCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RangeCollection‑metod. Lägger till ett Range‑objekt i samlingen"
type: docs
url: /sv/net/aspose.cells/rangecollection/add/
---
## RangeCollection.Add method

Lägger till ett [`Range`](../../range/)‑objekt i samlingen.

```csharp
[Obsolete("Use RangeCollection.AddRange(Range) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(Range range)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | Range | Range‑objekt |

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället AddRange()‑metoden. Denna metod kommer att tas bort 6 månader senare från och med december 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeCollectionMethodAddWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett intervall och lägg till det i samlingen
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // Infoga rader för att demonstrera att intervallet expanderar
            worksheet.Cells.InsertRows(2, 2);
            
            Console.WriteLine("Range row count after insertion: " + cellRange.RowCount);
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


