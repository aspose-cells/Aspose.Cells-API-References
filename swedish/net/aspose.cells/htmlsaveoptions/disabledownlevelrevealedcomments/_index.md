---
title: "HtmlSaveOptions.DisableDownlevelRevealedComments"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om Downlevelrevealed villkorliga kommentarer ska inaktiveras vid export av fil till html. Standardvärdet är falskt."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/
---
## HtmlSaveOptions.DisableDownlevelRevealedComments property

Anger om Downlevel‑revealed villkorliga kommentarer ska inaktiveras vid export av fil till html, standardvärdet är false.

```csharp
public bool DisableDownlevelRevealedComments { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyDisableDownlevelRevealedCommentsDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med en kommentar
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a test comment";

            // Ställ in HTML-sparalternativ med DisableDownlevelRevealedComments
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.DisableDownlevelRevealedComments = true;

            // Spara arbetsboken med HTML-alternativ
            workbook.Save("output.html", options);
            
            Console.WriteLine("Workbook saved with DisableDownlevelRevealedComments=true");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


