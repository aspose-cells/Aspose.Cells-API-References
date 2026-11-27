---
title: "Style.IsTextWrapped"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Hämtar eller anger ett värde som indikerar om texten i en cell är radbruten"
type: docs
url: /sv/net/aspose.cells/style/istextwrapped/
---
## Style.IsTextWrapped property

Hämtar eller anger ett värde som indikerar om texten i en cell är radbruten.

```csharp
public bool IsTextWrapped { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;
            
            // Ställ in lång text i cellen
            Cell cell = cells["A1"];
            cell.PutValue("This is a long text that should be wrapped in the cell");
            
            // Aktivera radbrytning av text
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;
            cell.SetStyle(style);
            
            // Justera radhöjden för att visa radbruten text
            ws.AutoFitRow(0);
            
            // Spara arbetsboken
            wb.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


