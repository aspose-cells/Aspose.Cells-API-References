---
title: "HtmlSaveOptions.IsExpImageToTempDir"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om bildfiler exporteras till temporär katalog. Endast för sparande till html-ström"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/isexpimagetotempdir/
---
## HtmlSaveOptions.IsExpImageToTempDir property

Anger om bildfiler ska exporteras till en temporär katalog. Endast för att spara till HTML-ström.

```csharp
public bool IsExpImageToTempDir { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsExpImageToTempDirDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med en bild
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en exempelbild i kalkylbladet
            worksheet.Pictures.Add(0, 0, "https://www.aspose.com/templates/aspose/App_Themes/V3/images/cells/header/aspose_cells-for-net.png");

            // Ställ in HTML-sparalternativ med IsExpImageToTempDir aktiverat
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.IsExpImageToTempDir = true;
            options.ExportImagesAsBase64 = false; // Ensure images are exported as separate files

            // Spara arbetsboken som HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML saved with images exported to temp directory.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


