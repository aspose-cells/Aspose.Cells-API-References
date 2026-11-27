---
title: "HtmlSaveOptions.DefaultFontName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions‑egenskap. Ange standardtypsnamsnamnet för export av html. Standardtypsnittet kommer att användas när stilens typsnitt inte finns. Om denna egenskap är null kommer Aspose.Cells att använda ett universellt typsnitt som har samma familj som originaltypsnittet. Standardvärdet är null"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/defaultfontname/
---
## HtmlSaveOptions.DefaultFontName property

Ange standardteckensnittets namn för export av html, standardteckensnittet används när stilens teckensnitt inte finns. Om denna egenskap är null kommer Aspose.Cells att använda ett universellt teckensnitt som har samma familj som originalteckensnittet, standardvärdet är null.

```csharp
public string DefaultFontName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyDefaultFontNameDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // Ställ in HTML‑sparalternativ med anpassat standardtypsnitt
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.DefaultFontName = "Courier New";
            
            // Spara till HTML med det angivna typsnittet
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with default font: " + saveOptions.DefaultFontName);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


