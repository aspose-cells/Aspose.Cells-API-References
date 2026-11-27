---
title: "Range.EntireColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-egenskapen. Hämtar ett Range-objekt som representerar hela kolumnen eller kolumnerna som innehåller det angivna intervallet"
type: docs
url: /sv/net/aspose.cells/range/entirecolumn/
---
## Range.EntireColumn property

Hämtar ett Range-objekt som representerar hela kolumnen (eller kolumnerna) som innehåller det angivna området.

```csharp
public Range EntireColumn { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett intervall som börjar vid cell C1 (rad 0, kolumn 2)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, 1, 1);
            
            // Hämta hela kolumnen som innehåller intervallet (kolumn C)
            Aspose.Cells.Range entireColumn = range.EntireColumn;
            
            // Applicera formatering på hela kolumnen
            Style style = entireColumn[0, 0].GetStyle();
            style.Custom = "##0%";
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            entireColumn.ApplyStyle(style, styleFlag);
            
            // Spara arbetsboken
            workbook.Save("EntireColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


