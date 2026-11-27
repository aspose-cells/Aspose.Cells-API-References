---
title: "HtmlSaveOptions.HideOverflowWrappedText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions‑egenskap. Anger om överskjutande text ska döljas när cellformatet är inställt på att radbryta text. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/
---
## HtmlSaveOptions.HideOverflowWrappedText property

Anger om överskjutande text ska döljas när cellformatet är inställt på radbrytning. Standardvärdet är false

```csharp
public bool HideOverflowWrappedText { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHideOverflowWrappedTextDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in exempeltext i cell A1
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap and hide overflow when exported to HTML");
            
            // Skapa och tillämpa stil med textbrytning
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // Hämta cellsamlingen och tillämpa stil
            Cells cells = worksheet.Cells;
            cells["A1"].SetStyle(style, flag);
            
            // Ställ in kolumnbredd för att få texten att radbrytas
            cells.SetColumnWidth(0, 10);
            
            // Skapa HTML‑sparalternativ och ställ in HideOverflowWrappedText
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HideOverflowWrappedText = true;
            
            // Spara arbetsbok med HTML-alternativ
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved with HideOverflowWrappedText: " + outputPath);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


