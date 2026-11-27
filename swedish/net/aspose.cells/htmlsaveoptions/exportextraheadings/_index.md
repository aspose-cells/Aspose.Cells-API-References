---
title: "HtmlSaveOptions.ExportExtraHeadings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om extra rubriker exporteras när textens längd är längre än max visningskolumn. Standardvärdet är false. Om du vill importera html-filen till Excel, behåll standardvärdet"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportextraheadings/
---
## HtmlSaveOptions.ExportExtraHeadings property

Anger om extra rubriker ska exporteras när textlängden är längre än den maximala visningskolumnen. Standardvärdet är false. Om du vill importera html-filen till Excel, behåll standardvärdet.

```csharp
public bool ExportExtraHeadings { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportExtraHeadingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och extra rubriker
            worksheet.Cells["A1"].PutValue("Main Heading");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue("Data3");
            worksheet.Cells["B3"].PutValue("Data4");
            
            // Ställ in extra rubriker (rader och kolumner)
            worksheet.Cells["Z1"].PutValue("Extra Column Heading");
            worksheet.Cells["A100"].PutValue("Extra Row Heading");

            // Konfigurera HTML-sparalternativ med ExportExtraHeadings
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportHeadings = true;
            saveOptions.ExportExtraHeadings = true;

            // Spara till HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML exported with extra headings.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


