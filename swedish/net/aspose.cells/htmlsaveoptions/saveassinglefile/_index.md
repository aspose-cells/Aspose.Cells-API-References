---
title: "HtmlSaveOptions.SaveAsSingleFile"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions‑egenskap. Anger om HTML ska sparas som en enda fil. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/saveassinglefile/
---
## HtmlSaveOptions.SaveAsSingleFile property

Anger om HTML ska sparas som en enda fil. Standardvärdet är falskt.

```csharp
public bool SaveAsSingleFile { get; set; }
```

### Anmärkningar

Om det finns flera kalkylblad eller andra nödvändiga resurser, såsom bilder i arbetsboken, måste dessa kalkylblad och resurser vanligtvis sparas i separata filer. I vissa scenarier kan användaren behöva endast en resulterande fil för att underlätta överföring. I så fall kan användaren sätta denna egenskap till true.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertySaveAsSingleFileDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Initiera HTML‑sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.SaveAsSingleFile = true;
            saveOptions.ExportPageHeaders = true;
            
            // Spara arbetsboken som en enda HTML‑fil
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            // Verifiera att utdatafilen finns
            if (File.Exists(outputPath))
            {
                Console.WriteLine("HTML saved as single file successfully.");
            }
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


