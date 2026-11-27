---
title: "HtmlSaveOptions.HiddenRowDisplayType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Dolda rader – höjden på denna rad är 0 i Excel. Innan du sparar till HTML-format, om HtmlHiddenRowDisplayType är Remove så kommer dolda rader inte att skrivas ut; om värdet är Hidden så kommer raden att skrivas ut men vara dold. Standardvärdet är Hidden."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/
---
## HtmlSaveOptions.HiddenRowDisplayType property

Dold rad (höjden på den här raden är 0) i Excel, innan du sparar detta i HTML-format, om HtmlHiddenRowDisplayType är "Remove" kommer den dolda raden inte att skrivas ut, om värdet är "Hidden" kommer raden att skrivas ut men vara dold, standardvärdet är "Hidden"

```csharp
public HtmlHiddenRowDisplayType HiddenRowDisplayType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenRowDisplayTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och dölj en rad
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row");
            worksheet.Cells.HideRow(1); // Hide row 2 (0-based index 1)

            // Ställ in HTML-sparalternativ med HiddenRowDisplayType
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;

            // Spara till HTML
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with hidden rows handled according to HiddenRowDisplayType setting.");
        }
    }
}
```

### Se även

* enum [HtmlHiddenRowDisplayType](../../htmlhiddenrowdisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


