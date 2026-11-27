---
title: "HtmlSaveOptions.ParseHtmlTagInCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om HTML-taggar såsom div/div i cellen ska tolkas som cellvärde eller bevaras som de är. Standardvärdet är sant."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/parsehtmltagincell/
---
## HtmlSaveOptions.ParseHtmlTagInCell property

Anger om HTML-taggar (såsom `<div></div>`) i en cell ska tolkas som cellvärde eller bevaras som de är. Standardvärdet är true.

```csharp
public bool ParseHtmlTagInCell { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyParseHtmlTagInCellDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata som innehåller HTML-taggar
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in cellvärde med HTML-taggar
            worksheet.Cells["A1"].PutValue("<b>Bold Text</b> and <i>Italic Text</i>");
            
            // Skapa HTML-sparalternativ och aktivera tolkning av HTML-taggar
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            htmlSaveOptions.ParseHtmlTagInCell = true;
            
            // Spara arbetsboken med tolkade HTML-taggar
            workbook.Save("output.html", htmlSaveOptions);
            
            Console.WriteLine("HTML saved with ParseHtmlTagInCell enabled.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


