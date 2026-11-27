---
title: "HtmlSaveOptions.ExportPrintAreaOnly"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions‑egenskap. Anger om endast utskriftsområdet exporteras till html‑fil. Standardvärdet är falskt"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportprintareaonly/
---
## HtmlSaveOptions.ExportPrintAreaOnly property

Anger om endast utskriftsområdet ska exporteras till html-fil. Standardvärdet är false.

```csharp
public bool ExportPrintAreaOnly { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPrintAreaOnlyDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange exempeldata
            for (int i = 0; i < 20; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            // Ställ in utskriftsområde
            worksheet.PageSetup.PrintArea = "B2:F10";

            // Konfigurera HTML‑sparalternativ
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportPrintAreaOnly = true;
            options.ExportGridLines = true;

            // Spara arbetsboken med endast utskriftsområde
            workbook.Save("output.html", options);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


