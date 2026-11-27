---
title: "HtmlSaveOptions.FormatDataIgnoreColumnWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om hela den formaterade cellens data ska visas när den överflödar kolumnen. Om true ignoreras kolumnbredden och hela cellens data exporteras. Om false exporteras data på samma sätt som i Excel. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/
---
## HtmlSaveOptions.FormatDataIgnoreColumnWidth property

Anger om hela den formaterade celldata ska visas när den överskrider kolumnen. Om true ignoreras kolumnbredden och hela cellens data exporteras. Om false exporteras data på samma sätt som i Excel. Standardvärdet är false.

```csharp
public bool FormatDataIgnoreColumnWidth { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFormatDataIgnoreColumnWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in exempeldata och kolumnbredd
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B1"].PutValue("Longer Text That Might Be Truncated");
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 5);  // Very narrow column

            // Skapa HTML-sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Demonstrera egenskapen FormatDataIgnoreColumnWidth
            saveOptions.FormatDataIgnoreColumnWidth = true; // Text won't be truncated by column width
            
            // Spara med olika inställningar för att visa effekten
            workbook.Save("HtmlWithIgnoreColumnWidth.html", saveOptions);
            
            saveOptions.FormatDataIgnoreColumnWidth = false; // Text may be truncated by column width
            workbook.Save("HtmlWithoutIgnoreColumnWidth.html", saveOptions);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


