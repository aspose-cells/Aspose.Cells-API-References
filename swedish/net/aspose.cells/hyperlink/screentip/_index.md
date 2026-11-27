---
title: "Hyperlink.ScreenTip"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Hyperlink‑egenskap. Returnerar eller anger ScreenTip‑texten för den angivna hyperlänken"
type: docs
url: /sv/net/aspose.cells/hyperlink/screentip/
---
## Hyperlink.ScreenTip property

Returnerar eller anger ScreenTip‑texten för den angivna hyperlänken.

```csharp
public string ScreenTip { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyScreenTipDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Click this hyperlink:");

            // Skapa en hyperlänk med ScreenTip
            int hLinkIdx = worksheet.Hyperlinks.Add("B1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks[hLinkIdx].ScreenTip = "Visit Aspose website for more information";

            // Spara arbetsboken
            workbook.Save("HyperlinkWithScreenTip.xlsx");
        }
    }
}
```

### Se även

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


