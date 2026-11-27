---
title: "HtmlSaveOptions.ExportBogusRowData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions‑egenskap. Anger om falsk nedersta raddata ska exporteras. Standardvärdet är true. Om du vill importera html‑ eller mht‑filen till Excel, behåll standardvärdet."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportbogusrowdata/
---
## HtmlSaveOptions.ExportBogusRowData property

Anger om falska data i den nedre raden ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet.

```csharp
public bool ExportBogusRowData { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportBogusRowDataDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite data i cellerna
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Skapa HTML-sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            
            // Första export utan falsk raddata
            saveOptions.ExportBogusRowData = false;
            workbook.Save("output_without_bogus.html", saveOptions);
            
            // Sedan export med falsk raddata
            saveOptions.ExportBogusRowData = true;
            workbook.Save("output_with_bogus.html", saveOptions);

            // Visa resultaten
            Console.WriteLine("HTML files created successfully.");
            Console.WriteLine("Check output_without_bogus.html and output_with_bogus.html to see the difference.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


