---
title: "HtmlSaveOptions.DisableDownlevelRevealedComments"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob Downlevelrevealed bedingte Kommentare beim Exportieren der Datei nach HTML deaktiviert werden; der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/
---
## HtmlSaveOptions.DisableDownlevelRevealedComments property

Gibt an, ob Downlevel‑revealed bedingte Kommentare beim Exportieren der Datei nach HTML deaktiviert werden sollen, der Standardwert ist false.

```csharp
public bool DisableDownlevelRevealedComments { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyDisableDownlevelRevealedCommentsDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispiel-Arbeitsmappe mit einem Kommentar
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a test comment";

            // Setze HTML-Speicheroptionen mit DisableDownlevelRevealedComments
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.DisableDownlevelRevealedComments = true;

            // Speichere die Arbeitsmappe mit HTML-Optionen
            workbook.Save("output.html", options);
            
            Console.WriteLine("Workbook saved with DisableDownlevelRevealedComments=true");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


