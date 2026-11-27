---
title: "PageSetup.SetFooter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Ställer in ett skript som formaterar sidfoten i en Excel-fil"
type: docs
url: /sv/net/aspose.cells/pagesetup/setfooter/
---
## PageSetup.SetFooter method

Ställer in ett skript som formaterar sidfoten i en Excel-fil.

```csharp
public void SetFooter(int section, string footerScript)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sektion | Int32 | 0: Vänster sektion, 1: Centrerad sektion, 2: Höger sektion. |
| footerScript | String | Sidfotformatskript. |

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

Till exempel: "&amp;Arial,Bold&amp;8Footer Note"

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.SetFooter(0, "Page &P");
            worksheet.PageSetup.SetFooter(1, "&D");
            worksheet.PageSetup.SetFooter(2, "&A");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


