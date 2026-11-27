---
title: "HtmlSaveOptions.ImageScalable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om skalbar enhet används för att beskriva bildens bredd när skalbar enhet används för att beskriva kolumnens bredd. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/imagescalable/
---
## HtmlSaveOptions.ImageScalable property

Anger om en skalbar enhet ska användas för att beskriva bildens bredd när en skalbar enhet används för att beskriva kolumnens bredd. Standardvärdet är true.

```csharp
public bool ImageScalable { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyImageScalableDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med en bild
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en exempelbild i kalkylbladet
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[imgIndex];

            // Ställ in HTML-sparalternativ med ImageScalable-egenskapen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ImageScalable = false; // Images won't scale with the HTML content
            
            // Spara arbetsboken som HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with ImageScalable set to false.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


