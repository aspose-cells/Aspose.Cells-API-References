---
title: "HtmlSaveOptions.PageTitle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Titeln på html-sidan. Endast för sparande till html-ström"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/pagetitle/
---
## HtmlSaveOptions.PageTitle property

Titeln på HTML-sidan. Endast för att spara till HTML-ström.

```csharp
public string PageTitle { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyPageTitleDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");

            // Ställ in HTML-sparalternativ med PageTitle
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.PageTitle = "My Custom Page Title";

            // Spara till HTML med den angivna titeln
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with custom page title: " + outputPath);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


