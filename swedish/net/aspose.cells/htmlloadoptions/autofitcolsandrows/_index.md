---
title: "HtmlLoadOptions.AutoFitColsAndRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlLoadOptions egenskap. Anger om autofit av kolumner och rader. Standardvärdet är falskt"
type: docs
url: /sv/net/aspose.cells/htmlloadoptions/autofitcolsandrows/
---
## HtmlLoadOptions.AutoFitColsAndRows property

Anger om kolumner och rader ska auto-anpassas. Standardvärdet är falskt.

```csharp
public bool AutoFitColsAndRows { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAutoFitColsAndRowsDemo
    {
        public static void Run()
        {
            // Skapa HTML‑laddningsalternativ
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // Aktivera automatisk anpassning av kolumner och rader
            loadOptions.AutoFitColsAndRows = true;
            
            // Läs in HTML-fil med de angivna alternativen
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Automatisk anpassning av kolumner och rader kommer att tillämpas vid inläsning
            Console.WriteLine("Columns and rows have been auto-fitted during HTML import.");
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


