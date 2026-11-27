---
title: "Range.CopyStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Kopierar stilinställningar från ett källområde"
type: docs
url: /sv/net/aspose.cells/range/copystyle/
---
## Range.CopyStyle method

Kopierar stilinställningar från ett källområde.

```csharp
public void CopyStyle(Range range)
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
    public class RangeMethodCopyStyleWithRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            
            // Lägg till ett exempel på stil i källområdet
            Cells cellsSrc = sheetSrc.Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A1:D5");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            rangeSrc.SetStyle(style);
            
            // Skapa destinationsarbetsblad
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";
            
            // Skapa destinationsområde och kopiera stil
            Cells cellsDest = sheetDest.Cells;
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange("A1:D5");
            rangeDest.CopyStyle(rangeSrc);
            
            // Spara arbetsboken
            workbook.Save("RangeCopyStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


