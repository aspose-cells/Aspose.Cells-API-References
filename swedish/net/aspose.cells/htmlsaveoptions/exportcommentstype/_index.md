---
title: "HtmlSaveOptions.ExportCommentsType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Representerar typ av export av kommentarer till html-filer"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportcommentstype/
---
## HtmlSaveOptions.ExportCommentsType property

Representerar typ av export av kommentarer till html-filer.

```csharp
public PrintCommentsType ExportCommentsType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportCommentsTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempelkommentar med cellnamn
            Comment comment = worksheet.Comments["A1"];
            comment.Note = "This is a test comment";
            
            // Ställ in HTML‑sparalternativ med ExportCommentsType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportCommentsType = PrintCommentsType.PrintInPlace;
            
            // Spara till HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file with comments exported successfully.");
        }
    }
}
```

### Se även

* enum [PrintCommentsType](../../printcommentstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


