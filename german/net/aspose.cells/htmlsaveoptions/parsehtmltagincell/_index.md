---
title: "HtmlSaveOptions.ParseHtmlTagInCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions property. Gibt an, ob HTML-Tags wie div/div in einer Zelle als Zellenwert geparst oder unverändert beibehalten werden sollen. Der Standardwert ist true"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/parsehtmltagincell/
---
## HtmlSaveOptions.ParseHtmlTagInCell property

Gibt an, ob HTML‑Tags (wie `<div></div>`) in einer Zelle als Zellenwert geparst oder unverändert beibehalten werden sollen. Der Standardwert ist true.

```csharp
public bool ParseHtmlTagInCell { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyParseHtmlTagInCellDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe mit Beispieldaten, die HTML-Tags enthalten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze den Zellenwert mit HTML-Tags
            worksheet.Cells["A1"].PutValue("<b>Bold Text</b> and <i>Italic Text</i>");
            
            // Erstelle HTML-Speicheroptionen und aktiviere das Parsen von HTML-Tags
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            htmlSaveOptions.ParseHtmlTagInCell = true;
            
            // Speichere die Arbeitsmappe mit geparsten HTML-Tags
            workbook.Save("output.html", htmlSaveOptions);
            
            Console.WriteLine("HTML saved with ParseHtmlTagInCell enabled.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


