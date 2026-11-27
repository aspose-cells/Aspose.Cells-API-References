---
title: "HtmlLoadOptions.LoadFormulas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlLoadOptions-egenskapen. Anger om formler ska importeras om den ursprungliga HTML‑filen innehåller formler"
type: docs
url: /sv/net/aspose.cells/htmlloadoptions/loadformulas/
---
## HtmlLoadOptions.LoadFormulas property

Anger om formler ska importeras om den ursprungliga html-filen innehåller formler

```csharp
public bool LoadFormulas { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyLoadFormulasDemo
    {
        public static void Run()
        {
            // Skapa en instans av HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Ställ in LoadFormulas till true för att ladda formler från HTML
            loadOptions.LoadFormulas = true;

            // Ladda en HTML‑fil som innehåller formler till en arbetsbok
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Visa formeln från cell A1 (om den finns i HTML)
            Console.WriteLine("Formula in A1: " + worksheet.Cells["A1"].Formula);

            // Spara arbetsboken till en Excel-fil
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


