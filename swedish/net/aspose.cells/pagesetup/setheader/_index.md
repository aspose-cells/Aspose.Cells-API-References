---
title: "PageSetup.SetHeader"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Ställer in ett skript som formaterar sidhuvudet i en Excel-fil"
type: docs
url: /sv/net/aspose.cells/pagesetup/setheader/
---
## PageSetup.SetHeader method

Ställer in ett skript som formaterar sidhuvudet i en Excel-fil.

```csharp
public void SetHeader(int section, string headerScript)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sektion | Int32 | 0: Vänster sektion, 1: Centrerad sektion, 2: Höger sektion. |
| headerScript | String | Rubrikformatskript. |

### Anmärkningar

Skriptkommandon:

| **Kommando** | **Beskrivning** |
| --- | --- |
| &amp;P | Aktuellt sidnummer |
| &amp;N | Sidantal |
| &amp;D | Aktuellt datum |
| &amp;T | Aktuell tid |
| &amp;A | Bladnamn |
| &amp;F | Filnamn utan sökväg |
| &amp;\"&lt;FontName&gt;\" | Typsnittsnamn, till exempel: &amp;\"Arial\" |
| &amp;\"&lt;FontName&gt;, &lt;FontStyle&gt;\" | Typsnittsnamn och typsnittsstil, till exempel: &amp;\"Arial,Bold\" |
| &amp;&lt;FontSize&gt; | Typsnittsstorlek. Om detta kommando följs av ett vanligt tal som ska skrivas ut i rubriken, separeras det från teckenhöjden med ett mellanslag. |
| &amp;K&lt;RRGGBB&gt; | Typsnittsfärg, till exempel(RÖD): &amp;KFF0000 |
| &amp;G | Bildskript |

Till exempel: \"&amp;Arial,Bold&amp;8Header Note\"

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Ställ in olika rubriksektioner med olika kommandon
            pageSetup.SetHeader(0, "&F"); // Left section - File name
            pageSetup.SetHeader(1, "Page &P of &N"); // Center section - Page numbering
            pageSetup.SetHeader(2, "&D"); // Right section - Date

            workbook.Save("PageSetup_SetHeader_Example.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


