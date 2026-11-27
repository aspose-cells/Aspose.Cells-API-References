---
title: "Font.IsStrikeout"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font-egenskap. Hämtar eller anger ett värde som indikerar om fonten har enkel genomstrykning"
type: docs
url: /sv/net/aspose.cells/font/isstrikeout/
---
## Font.IsStrikeout property

Hämtar eller anger ett värde som indikerar om teckensnittet har enkel genomstrykning.

```csharp
public bool IsStrikeout { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsStrikeoutDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Metod 1: Ställ in genomstrykning via stil direkt
            Cell cell1 = worksheet.Cells["A1"];
            Style style1 = cell1.GetStyle();
            style1.Font.IsStrikeout = true;
            cell1.SetStyle(style1);
            cell1.PutValue("Strikeout Text (Style)");
            
            // Metod 2: Ställ in genomstrykning via HTML
            Cell cell2 = worksheet.Cells["A2"];
            cell2.HtmlString = "<s>Strikeout Text (HTML)</s>";
            
            // Verifiera genomstrykningsegenskapen
            Console.WriteLine("A1 IsStrikeout: " + cell1.GetStyle().Font.IsStrikeout);
            Console.WriteLine("A2 IsStrikeout: " + cell2.GetStyle().Font.IsStrikeout);
            
            // Spara för verifiering
            workbook.Save("FontStrikeoutDemo.xlsx");
        }
    }
}
```

### Se även

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


