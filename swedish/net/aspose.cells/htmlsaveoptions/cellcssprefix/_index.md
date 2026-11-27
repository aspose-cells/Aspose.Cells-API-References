---
title: "HtmlSaveOptions.CellCssPrefix"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Hämtar och anger prefixet för css-namnet. Standardvärdet är"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/cellcssprefix/
---
## HtmlSaveOptions.CellCssPrefix property

Hämtar och anger prefixet för css‑namnet, standardvärdet är "".

```csharp
public string CellCssPrefix { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCellCssPrefixDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Ställ in HTML-sparalternativ med CellCssPrefix
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.CellCssPrefix = "custom-cell-";

            // Spara arbetsboken med HTML-alternativ
            workbook.Save("output.html", saveOptions);

            Console.WriteLine("HTML file saved with custom cell CSS prefix.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


