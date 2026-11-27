---
title: "HtmlSaveOptions.ExportImagesAsBase64"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Anger om bilder sparas i Base64‑format till HTML, MHTML eller EPUB"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportimagesasbase64/
---
## HtmlSaveOptions.ExportImagesAsBase64 property

Anger om bilder sparas i Base64-format till HTML, MHTML eller EPUB.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Anmärkningar

När denna egenskap är satt till true exporteras bilddata direkt i img‑elementen och separata filer skapas inte.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en bild i kalkylbladet
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // Skapa HTML-sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Ställ in ExportImagesAsBase64 till true för att bädda in bilder som base64‑strängar
            saveOptions.ExportImagesAsBase64 = true;
            
            // Spara arbetsboken som HTML med inbäddade bilder
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML with embedded images saved successfully.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


