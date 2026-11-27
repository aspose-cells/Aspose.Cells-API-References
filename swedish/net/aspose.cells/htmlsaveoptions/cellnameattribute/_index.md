---
title: "HtmlSaveOptions.CellNameAttribute"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger attributet som indikerar CellName som ska skrivas. t.ex. Om värdet är id så blir utdata för cell A1 td idA1. Standardvärdet är null"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/cellnameattribute/
---
## HtmlSaveOptions.CellNameAttribute property

Anger attributet som visar CellName som ska skrivas. (t.ex. Om värdet är "id", så blir utskriften för cellen "A1" &lt;td id='A1'&gt;). Standardvärdet är null.

```csharp
public string CellNameAttribute { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using System.Text.RegularExpressions;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCellNameAttributeDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med lite data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["B2"].PutValue(123);

            // Ställ in HTML-sparalternativ med CellNameAttribute
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.CellNameAttribute = "id";
            saveOptions.ExportImagesAsBase64 = true;
            saveOptions.ExportActiveWorksheetOnly = true;

            // Spara till HTML‑fil
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            // Verifiera att HTML-utdata innehåller cell-ID:n
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains A1 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='A1'"));
            Console.WriteLine("HTML contains B2 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='B2'"));
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


