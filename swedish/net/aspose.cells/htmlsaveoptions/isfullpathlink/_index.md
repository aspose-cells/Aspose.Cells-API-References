---
title: "HtmlSaveOptions.IsFullPathLink"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Anger om fullständig sökvägslänk används i sheet00x.htmfilelist.xml och tabstrip.htm. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/isfullpathlink/
---
## HtmlSaveOptions.IsFullPathLink property

Anger om fullständig sökväg ska användas i länkar i sheet00x.htm, filelist.xml och tabstrip.htm. Standardvärdet är false.

```csharp
public bool IsFullPathLink { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsFullPathLinkDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test HTML Export");

            // Skapa HTML-sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Demonstrera IsFullPathLink egenskap
            saveOptions.IsFullPathLink = true; // Set to true to use full path links
            
            // Spara med olika IsFullPathLink-inställningar
            workbook.Save("HtmlExport_FullPathLinks.html", saveOptions);
            
            saveOptions.IsFullPathLink = false; // Set to false for relative paths
            workbook.Save("HtmlExport_RelativeLinks.html", saveOptions);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


