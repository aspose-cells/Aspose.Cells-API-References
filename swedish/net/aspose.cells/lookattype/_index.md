---
title: "Enum LookAtType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LookAtType enum. Representerar söktyp"
type: docs
url: /sv/net/aspose.cells/lookattype/
---
## LookAtType enumeration

Representerar typen för look at.

```csharp
public enum LookAtType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Contains | `0` | Cellvärde innehåller sökobjektet. |
| StartWith | `1` | Cellvärde börjar med sökobjektet. |
| EndWith | `2` | Cellvärde slutar med sökobjektet. |
| EntireContent | `3` | Cellvärde är samma som sökobjektet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LookAtTypeDemo
    {
        public static void LookAtTypeExample()
        {
            // Instansiera arbetsbokobjektet
            Workbook workbook = new Workbook("LookAtTypeExample_original.xlsx");

            // Hämta Cells-samlingen 
            Cells cells = workbook.Worksheets[0].Cells;

            // Instansiera FindOptions-objektet
            FindOptions findOptions = new FindOptions();

            // Skapa ett Cells-område
            CellArea ca = new CellArea();
            ca.StartRow = 8;
            ca.StartColumn = 2;
            ca.EndRow = 17;
            ca.EndColumn = 13;

            // Ställ in cellområdet för sökalternativ
            findOptions.SetRange(ca);

            // Ställ in sökegenskaper
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // Ställ in LookAtType till Contains
            findOptions.LookAtType = LookAtType.Contains;

            // Hitta cellen med ett specifikt värde
            Cell cell = cells.Find("searchValue", null, findOptions);

            if (cell != null)
            {
                Console.WriteLine($"Cell found at row {cell.Row}, column {cell.Column}");
            }
            else
            {
                Console.WriteLine("Cell not found.");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


