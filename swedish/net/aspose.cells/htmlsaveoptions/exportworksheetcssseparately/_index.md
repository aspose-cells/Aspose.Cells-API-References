---
title: "HtmlSaveOptions.ExportWorksheetCSSSeparately"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions‑egenskap. Anger om kalkylblad‑css ska exporteras separat. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportworksheetcssseparately/
---
## HtmlSaveOptions.ExportWorksheetCSSSeparately property

Anger om kalkylbladets CSS ska exporteras separat. Standardvärdet är false.

```csharp
public bool ExportWorksheetCSSSeparately { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorksheetCSSSeparatelyDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");
            
            // Ställ in HTML‑sparalternativ med ExportWorksheetCSSSeparately
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportWorksheetCSSSeparately = true;
            
            // Spara arbetsboken som HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file with separate CSS saved to: " + outputPath);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


