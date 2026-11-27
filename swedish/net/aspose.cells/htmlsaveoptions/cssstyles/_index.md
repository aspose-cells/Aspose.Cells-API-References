---
title: "HtmlSaveOptions.CssStyles"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Hämtar eller anger de extra css-stilarna för formateraren. Fungerar endast när SaveAsSingleFile är True.  CssStylesbody  padding 5px"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/cssstyles/
---
## HtmlSaveOptions.CssStyles property

Hämtar eller anger de extra css-stilarna för formateraren. Fungerar endast när [`SaveAsSingleFile`](../saveassinglefile/) är True.  CssStyles="body { padding: 5px }";

```csharp
public string CssStyles { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCssStylesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Skapa HTML-sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Ställ in anpassade CSS-stilar
            saveOptions.CssStyles = @"
                body { 
                    font-family: Arial;
                    background-color: #f0f0f0;
                }
                table {
                    border-collapse: collapse;
                    width: 100%;
                }
                td {
                    border: 1px solid #ddd;
                    padding: 8px;
                }";

            // Spara arbetsboken med anpassade CSS-stilar
            workbook.Save("HtmlWithCustomStyles.html", saveOptions);

            Console.WriteLine("HTML file with custom CSS styles created successfully.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


