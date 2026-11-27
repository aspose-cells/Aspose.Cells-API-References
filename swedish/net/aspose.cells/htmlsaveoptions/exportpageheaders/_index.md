---
title: "HtmlSaveOptions.ExportPageHeaders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions‑egenskap. Anger om sidhuvuden exporteras"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportpageheaders/
---
## HtmlSaveOptions.ExportPageHeaders property

Anger om sidhuvuden ska exporteras.

```csharp
public bool ExportPageHeaders { get; set; }
```

### Anmärkningar

Fungerar endast när [`SaveAsSingleFile`](../saveassinglefile/) är True.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPageHeadersDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in sidhuvud
            worksheet.PageSetup.SetHeader(0, "Sample Header Text");
            
            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("This is a test");
            
            // Konfigurera HTML‑sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                SaveAsSingleFile = true,
                ShowAllSheets = true,
                ExportPageHeaders = true  // This is the key property being demonstrated
            };
            
            // Spara arbetsboken som HTML
            string outputPath = "output_with_headers.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file with page headers exported successfully.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


