---
title: "HtmlSaveOptions.ExportDocumentProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om dokumentegenskaper ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportdocumentproperties/
---
## HtmlSaveOptions.ExportDocumentProperties property

Anger om dokumentegenskaper ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet.

```csharp
public bool ExportDocumentProperties { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till några dokumentegenskaper
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Lägg till exempelcelldata
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Skapa HTML-sparalternativ och sätt ExportDocumentProperties till false
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportDocumentProperties = false;
            
            // Spara arbetsboken som HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with document properties export disabled.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


