---
title: "Range.CopyValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metoden. Kopierar cellvärde från ett källintervall"
type: docs
url: /sv/net/aspose.cells/range/copyvalue/
---
## Range.CopyValue method

Kopierar cellvärde från ett källområde.

```csharp
public void CopyValue(Range range)
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
    public class RangeMethodCopyValueWithRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och hämta det första kalkylbladet
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "SourceSheet";
            
            // Lägg till ett annat arbetsblad för destinationen
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "DestinationSheet";
            
            // Skapa exempeldata i källintervallet
            Cells cellsSrc = sheetSrc.Cells;
            cellsSrc["A1"].PutValue("Source Data");
            cellsSrc["A2"].PutValue(10);
            cellsSrc["B2"].PutValue(20);
            cellsSrc["A3"].PutValue(30);
            cellsSrc["B3"].PutValue(40);
            
            // Skapa intervall för källa och destination
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A2:B3");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("D2:E3");
            
            // Kopiera värden från källintervallet till destinationsintervallet
            rangeDest.CopyValue(rangeSrc);
            
            // Spara arbetsboken
            workbook.Save("RangeCopyValueDemo.xlsx");
            
            Console.WriteLine("Values copied successfully from source range to destination range.");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


