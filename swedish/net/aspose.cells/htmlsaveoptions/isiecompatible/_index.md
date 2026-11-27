---
title: "HtmlSaveOptions.IsIECompatible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om den genererade HTML:en är kompatibel med IE-webbläsaren. Standardvärdet är falskt."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/isiecompatible/
---
## HtmlSaveOptions.IsIECompatible property

Anger om den genererade HTML-koden är kompatibel med IE-webbläsaren. Standardvärdet är false.

```csharp
public bool IsIECompatible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsIECompatibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("HTML Export Demo");

            // Skapa HTML-sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Ställ in IsIECompatible-egenskapen
            saveOptions.IsIECompatible = false; // Disable IE compatibility mode
            
            // Spara arbetsboken med HTML-alternativ
            workbook.Save("HtmlExportDemo.html", saveOptions);

            Console.WriteLine("HTML file saved with IsIECompatible = false");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


