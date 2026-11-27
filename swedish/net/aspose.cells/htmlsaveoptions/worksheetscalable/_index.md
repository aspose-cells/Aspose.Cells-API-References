---
title: "HtmlSaveOptions.WorksheetScalable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions property. Anger om zoomning in eller out av HTML via kalkylbladszoomnivå när filen sparas till HTML. Standardvärdet är false."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/worksheetscalable/
---
## HtmlSaveOptions.WorksheetScalable property

Anger om HTML zoomas in eller ut via kalkylbladets zoomnivå när filen sparas till HTML, standardvärdet är falskt.

```csharp
public bool WorksheetScalable { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWorksheetScalableDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Ställ in HTML‑sparalternativ med WorksheetScalable‑egenskapen
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WorksheetScalable = true;
            
            // Spara arbetsboken med HTML-alternativ
            string outputPath = "output.html";
            workbook.Save(outputPath, options);
            
            // Verifiera att utdata innehåller skalningsstil
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains scaling: " + htmlContent.Contains("transform: scale"));
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


