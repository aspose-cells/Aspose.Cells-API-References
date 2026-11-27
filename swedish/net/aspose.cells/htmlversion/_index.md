---
title: "Enum HtmlVersion"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HtmlVersion‑enum. Anger vilken HTML‑version som används vid sparande till HTML‑format."
type: docs
url: /sv/net/aspose.cells/htmlversion/
---
## HtmlVersion enumeration

Anger vilken version av HTML som används när man sparar till HTML-format.

```csharp
public enum HtmlVersion
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Default | `0` | Spara dokumentet i enlighet med MS Excel export av HTML. |
| XHtml | `1` | Sparar dokumentet i enlighet med XHTML 1.0 Transitional-standarden. |
| Html5 | `2` | Sparar dokumentet i enlighet med HTML 5-standarden. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHtmlVersionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion usage");

            // Skapa HTML-sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();

            // Ställ in HTML-version till HTML5
            saveOptions.HtmlVersion = HtmlVersion.Html5;

            // Spara arbetsboken med HTML5-version
            workbook.Save("HtmlVersionDemo_Html5.html", saveOptions);

            // Ändra HTML-version till XHTML
            saveOptions.HtmlVersion = HtmlVersion.XHtml;

            // Spara arbetsboken med XHTML-version
            workbook.Save("HtmlVersionDemo_XHtml.html", saveOptions);

            // Ställ in HTML-version till Standard (MS Excel-kompatibel)
            saveOptions.HtmlVersion = HtmlVersion.Default;

            // Spara arbetsboken med standardversion
            workbook.Save("HtmlVersionDemo_Default.html", saveOptions);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


