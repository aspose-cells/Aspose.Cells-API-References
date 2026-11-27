---
title: "HtmlSaveOptions.ExportRowColumnHeadings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om bladens rad- och kolumnrubriker exporteras när du sparar till HTML-filer"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportrowcolumnheadings/
---
## HtmlSaveOptions.ExportRowColumnHeadings property

Anger om bladets rad- och kolumnrubriker ska exporteras när man sparar till HTML-filer.

```csharp
public bool ExportRowColumnHeadings { get; set; }
```

### Anmärkningar

Standardvärdet är falskt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportRowColumnHeadingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);

            // Skapa HTML-sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Ställ in ExportRowColumnHeadings till false (standard är true)
            saveOptions.ExportRowColumnHeadings = false;

            // Spara arbetsboken med rubriker inaktiverade
            workbook.Save("output_without_headings.html", saveOptions);

            // Aktivera nu rubriker och spara igen
            saveOptions.ExportRowColumnHeadings = true;
            workbook.Save("output_with_headings.html", saveOptions);

            Console.WriteLine("HTML files saved with different heading visibility settings.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


