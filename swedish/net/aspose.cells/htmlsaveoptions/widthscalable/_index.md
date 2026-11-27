---
title: "HtmlSaveOptions.WidthScalable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Anger om kolumnbredd ska exporteras i skalenhet till html. Standardvärdet är falskt"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/widthscalable/
---
## HtmlSaveOptions.WidthScalable property

Anger om kolumnbredd exporteras i skalenhet till HTML. Standardvärdet är falskt.

```csharp
public bool WidthScalable { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWidthScalableDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test WidthScalable Property");
            worksheet.Cells["B1"].PutValue(123.45);
            
            // Ställ in HTML-sparalternativ med WidthScalable-egenskapen
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WidthScalable = true; // Demonstrate setting to true
            
            // Spara med skalbar bredd
            workbook.Save("output_scalable.html", options);
            
            // Spara igen med fast bredd
            options.WidthScalable = false;
            workbook.Save("output_fixed.html", options);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


