---
title: "HtmlSaveOptions.ExportHeadings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om bladens rad- och kolumnrubriker exporteras när du sparar till HTML-filer"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportheadings/
---
## HtmlSaveOptions.ExportHeadings property

Anger om bladets rad- och kolumnrubriker ska exporteras när man sparar till HTML-filer.

```csharp
[Obsolete("Use HtmlSaveOptions.ExportRowColumnHeadings instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExportHeadings { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd i stället egenskapen HtmlSaveOptions.ExportRowColumnHeadings. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportHeadingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Skapa HTML-sparalternativ och aktivera export av rubriker
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportHeadings = true;

            // Spara som HTML med rubriker
            workbook.Save("output_with_headings.html", options);
            
            // Spara igen utan rubriker för jämförelse
            options.ExportHeadings = false;
            workbook.Save("output_without_headings.html", options);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


