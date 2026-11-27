---
title: "HtmlSaveOptions.AttachedFilesUrlPrefix"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Ange URL-prefixet för bifogade filer, såsom bild, i html-filen. Endast för sparande till html-ström"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/attachedfilesurlprefix/
---
## HtmlSaveOptions.AttachedFilesUrlPrefix property

Ange Url‑prefixet för bifogade filer, såsom bild i html‑filen. Endast för att spara till html‑ström.

```csharp
public string AttachedFilesUrlPrefix { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAttachedFilesUrlPrefixDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test HTML Export");

            // Ställ in HTML‑sparalternativ med AttachedFilesUrlPrefix
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.AttachedFilesUrlPrefix = "www.aspose.com";

            // Spara arbetsboken med HTML-alternativ
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with AttachedFilesUrlPrefix: " + saveOptions.AttachedFilesUrlPrefix);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


