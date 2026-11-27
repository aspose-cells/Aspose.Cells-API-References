---
title: "HtmlSaveOptions.AddGenericFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Anger om en generisk teckensnitt ska läggas till i CSS‑font-family. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/addgenericfont/
---
## HtmlSaveOptions.AddGenericFont property

Anger om en generisk teckensnitt ska läggas till i CSS font-family. Standardvärdet är true

```csharp
public bool AddGenericFont { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAddGenericFontDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in exempeltext med ett specifikt teckensnitt
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            Style style = cell.GetStyle();
            style.Font.Name = "Pacifico";
            cell.SetStyle(style);

            // Spara med AddGenericFont aktiverat (standard)
            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
            workbook.Save("output_with_generic.html", options);

            // Spara med AddGenericFont inaktiverat
            options.AddGenericFont = false;
            workbook.Save("output_without_generic.html", options);

            // Verifiera resultaten
            string withGeneric = File.ReadAllText("output_with_generic.html");
            string withoutGeneric = File.ReadAllText("output_without_generic.html");

            Console.WriteLine("With generic font: " + (withGeneric.Contains("font-family:Pacifico,sans-serif") ? "Found" : "Not found"));
            Console.WriteLine("Without generic font: " + (withoutGeneric.Contains("font-family:Pacifico,sans-serif") ? "Found" : "Not found"));
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


