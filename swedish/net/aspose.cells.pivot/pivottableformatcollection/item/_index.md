---
title: "PivotTableFormatCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTableFormatCollection egenskap. Hämtar formatet efter indexet"
type: docs
url: /sv/net/aspose.cells.pivot/pivottableformatcollection/item/
---
## PivotTableFormatCollection indexer

Hämtar formatet efter indexet.

```csharp
public PivotTableFormat this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("example.xlsx");

            // Uppdatera alla pivottabeller
            workbook.Worksheets.RefreshAll();
            Cells cells = workbook.Worksheets[0].Cells;

            // Åtkomst till den första pivottabellen
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];

            // Demonstrera Item‑egenskapen genom att komma åt den första PivotFormat
            pt.PivotFormats[0].PivotArea.OnlyData = false;
            workbook.Worksheets.RefreshAll();

            // Ändra formatinställningar med hjälp av Item‑egenskapen
            pt.PivotFormats[0].PivotArea.OnlyLabel = true;
            workbook.Worksheets.RefreshAll();

            // Spara den modifierade arbetsboken
            workbook.Save("modified_example.xlsx");
        }
    }
}
```

### Se även

* class [PivotTableFormat](../../pivottableformat/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


