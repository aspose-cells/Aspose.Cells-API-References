---
title: "HtmlSaveOptions.MergeEmptyTdType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Alternativet för att slå ihop intilliggande tomma cell‑td‑element. Standardvärdet är MergeEmptyTdType.Default"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/mergeemptytdtype/
---
## HtmlSaveOptions.MergeEmptyTdType property

Alternativet att slå ihop intilliggande tomma celler (tomma td-element). Standardvärdet är MergeEmptyTdType.Default.

```csharp
public MergeEmptyTdType MergeEmptyTdType { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyMergeEmptyTdTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange exempeldata
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue(""); // Empty cell

            // Konfigurera HTML-sparalternativ med MergeEmptyTdType
            HtmlSaveOptions htmlOptions = new HtmlSaveOptions()
            {
                MergeEmptyTdType = MergeEmptyTdType.None // Demonstrate the property
            };

            // Spara till HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, htmlOptions);

            Console.WriteLine("HTML saved with MergeEmptyTdType.None. Output file: " + outputPath);
        }
    }
}
```

### Se även

* enum [MergeEmptyTdType](../../mergeemptytdtype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


