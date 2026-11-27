---
title: "HtmlLoadOptions.ProgId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlLoadOptions-egenskap. Hämtar program-id för att skapa filen. Endast för MHT-filer"
type: docs
url: /sv/net/aspose.cells/htmlloadoptions/progid/
---
## HtmlLoadOptions.ProgId property

Hämtar program‑id för att skapa filen. Gäller endast för MHT-filer.

```csharp
public string ProgId { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyProgIdDemo
    {
        public static void Run()
        {
            // Skapa HTML-laddningsalternativ med MHTML-format
            HtmlLoadOptions options = new HtmlLoadOptions(LoadFormat.MHtml);
            
            // Hämta ProgId-egenskapen
            Console.WriteLine("ProgId is: " + options.ProgId);

            // Skapa en annan instans och hämta dess ProgId
            HtmlLoadOptions wordOptions = new HtmlLoadOptions(LoadFormat.MHtml);
            Console.WriteLine("ProgId is: " + wordOptions.ProgId);
        }
    }
}
```

### Se även

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


