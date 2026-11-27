---
title: "HtmlSaveOptions.ExportWorkbookProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om arbetsboksegenskaper ska exporteras. Standardvärdet är true. Om du vill importera HTML‑ eller MHT‑filen till Excel, behåll standardvärdet"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportworkbookproperties/
---
## HtmlSaveOptions.ExportWorkbookProperties property

Anger om arbetsboks egenskaper ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet.

```csharp
public bool ExportWorkbookProperties { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorkbookPropertiesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till lite data i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Ställ in arbetsbokens egenskaper
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Title";

            // Skapa HTML-sparalternativ
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Demonstrera ExportWorkbookProperties genom att sätta den till false
            options.ExportWorkbookProperties = false;
            
            // Spara arbetsboken som HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with ExportWorkbookProperties set to false");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


