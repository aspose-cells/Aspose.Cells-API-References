---
title: "Range.CopyData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range‑metod. Kopierar celldata inklusive formler från ett källintervall"
type: docs
url: /sv/net/aspose.cells/range/copydata/
---
## Range.CopyData method

Kopierar celldata (inklusive formler) från ett källområde.

```csharp
public void CopyData(Range range)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | Range | Källa [`Range`](../) objekt. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyDataWithRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta det första kalkylbladet och lägg till några data
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            sheetSrc.Cells["A1"].PutValue("Source Data");
            sheetSrc.Cells["B1"].PutValue(100);
            sheetSrc.Cells["A2"].PutValue("More Data");
            sheetSrc.Cells["B2"].PutValue(200);

            // Lägg till ett destinationskalkylblad
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";

            // Skapa käll- och destinationsintervall
            Aspose.Cells.Range rangeSrc = sheetSrc.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("C3:D4");

            // Kopiera data från källintervall till destinationsintervall
            rangeDest.CopyData(rangeSrc);

            // Spara arbetsboken
            workbook.Save("RangeCopyDataDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


