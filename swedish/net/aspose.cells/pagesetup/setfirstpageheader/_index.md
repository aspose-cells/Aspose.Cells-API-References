---
title: "PageSetup.SetFirstPageHeader"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Ställer in ett skript som formaterar det första sidhuvudet i en Excel-fil. Påverkar endast i Excel 2007 när IsHFDiffFirst är sant"
type: docs
url: /sv/net/aspose.cells/pagesetup/setfirstpageheader/
---
## PageSetup.SetFirstPageHeader method

Ställer in ett skript som formaterar den första sidhuvudet i en Excel-fil. Endast effekt i Excel 2007 när IsHFDiffFirst är sant.

```csharp
public void SetFirstPageHeader(int section, string headerScript)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sektion | Int32 | 0: Vänster sektion, 1: Centrerad sektion, 2: Höger sektion. |
| headerScript | String | Rubrikformatskript. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFirstPageHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Ställ in första sidhuvudet med sektionsnummer och rubriktext
            pageSetup.SetFirstPageHeader(2, "&CHeader Text");

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


