---
title: "HtmlSaveOptions.ExportSingleTab"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om den enda fliken ska exporteras när filen bara har ett arbetsblad. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportsingletab/
---
## HtmlSaveOptions.ExportSingleTab property

Anger om den enda fliken ska exporteras när filen bara har ett kalkylblad. Standardvärdet är false.

```csharp
public bool ExportSingleTab { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportSingleTabDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa HTML-sparalternativ med ExportSingleTab satt till true
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportSingleTab = true,
                ExportImagesAsBase64 = true
            };

            // Spara arbetsboken som HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "SingleTabExport.html");
            workbook.Save(outputPath, options);

            Console.WriteLine("HTML file with single tab export created successfully: " + outputPath);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


