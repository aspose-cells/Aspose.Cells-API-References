---
title: "HtmlSaveOptions.ExportDataOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger regeln för export av HTML‑fildata. Standardvärdet är All"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportdataoptions/
---
## HtmlSaveOptions.ExportDataOptions property

Anger regeln för export av html-fildata. Standardvärdet är All.

```csharp
public HtmlExportDataOptions ExportDataOptions { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportDataOptionsDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa HTML‑sparalternativ och ange ExportDataOptions
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
            htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;

            // Spara som HTML med alla dataexportalternativ
            workbook.Save("output.html", htmlSaveOptions);

            Console.WriteLine("HTML file saved with ExportDataOptions.All");
        }
    }
}
```

### Se även

* enum [HtmlExportDataOptions](../../htmlexportdataoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


