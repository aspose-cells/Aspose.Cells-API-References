---
title: "HtmlSaveOptions.HtmlVersion"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger version av HTML-standarden som ska användas när HTML-formatet sparas. Standardvärdet är HtmlVersion.Default"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/htmlversion/
---
## HtmlSaveOptions.HtmlVersion property

Anger vilken version av HTML-standarden som ska användas när HTML-formatet sparas. Standardvärdet är HtmlVersion.Default.

```csharp
public HtmlVersion HtmlVersion { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyHtmlVersionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion property");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["C4"].PutValue("Sample Text");
            
            // Skapa en HtmlSaveOptions-instans
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Visa aktuellt HtmlVersion-värde
            Console.WriteLine("Current HtmlVersion: " + options.HtmlVersion);
            
            // Ställ in HtmlVersion till HTML5
            options.HtmlVersion = HtmlVersion.Html5;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // Spara med HTML5-version
            workbook.Save("HtmlVersion_Html5.html", options);
            
            // Byt till XHTML
            options.HtmlVersion = HtmlVersion.XHtml;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // Spara med XHTML-version
            workbook.Save("HtmlVersion_XHtml.html", options);
            
            // Återställ till standard
            options.HtmlVersion = HtmlVersion.Default;
            Console.WriteLine("HtmlVersion reset to: " + options.HtmlVersion);
            
            // Spara med standardversion
            workbook.Save("HtmlVersion_Default.html", options);
        }
    }
}
```

### Se även

* enum [HtmlVersion](../../htmlversion/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


