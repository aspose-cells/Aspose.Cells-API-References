---
title: "Range.AddHyperlink"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Lägger till en hyperlänk i en angiven cell eller ett område av celler"
type: docs
url: /sv/net/aspose.cells/range/addhyperlink/
---
## Range.AddHyperlink method

Lägger till en hyperlänk till en angiven cell eller ett cellområde.

```csharp
public Hyperlink AddHyperlink(string address, string textToDisplay, string screenTip)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| adress | String | Adress för hyperlänken. |
| textToDisplay | String | Texten som ska visas för den angivna hyperlänken. |
| screenTip | String | ScreenTip-texten för den angivna hyperlänken. |

### Returvärde

[`Hyperlink`](../../hyperlink/) object.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodAddHyperlinkWithStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:A5");
            
            // Lägg till hyperlänk med adress, visningstext och verktygstips
            range.AddHyperlink("https://www.aspose.com", "Visit Aspose", "Click to go to Aspose website");
            
            // Spara arbetsboken
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Se även

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


