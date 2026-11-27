---
title: "HtmlSaveOptions.ExportGridLines"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Anger om rutnätslinjer ska exporteras. Standardvärdet är falskt"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportgridlines/
---
## HtmlSaveOptions.ExportGridLines property

Anger om rutnät ska exporteras. Standardvärdet är false.

```csharp
public bool ExportGridLines { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportGridLinesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in rutnätslinjernas synlighet
            worksheet.IsGridlinesVisible = true;

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            worksheet.Cells["C3"].PutValue(DateTime.Now);

            // Skapa HTML-sparalternativ
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportGridLines = worksheet.IsGridlinesVisible,
                ExportActiveWorksheetOnly = true
            };

            // Spara som HTML
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with ExportGridLines: " + options.ExportGridLines);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


