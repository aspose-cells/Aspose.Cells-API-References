---
title: "ExternalLink.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalLink egenskap. Hämtar typen av extern länk"
type: docs
url: /sv/net/aspose.cells/externallink/type/
---
## ExternalLink.Type property

Hämtar typen av extern länk.

```csharp
public ExternalLinkType Type { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad
            Worksheet sheet = workbook.Worksheets[0];
            
            // Skapa en extern länk till en annan arbetsbok
            sheet.Cells["A1"].Formula = "='[link.xls]Sheet1'!A1";
            
            // Hämta den externa länken
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // Visa typen av extern länk
            Console.WriteLine("External Link Type: " + externalLink.Type);
            
            // Ändra den externa länkens datakälla
            externalLink.DataSource = "d:\\link.xls";
            
            // Spara arbetsboken
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }
}
```

### Se även

* enum [ExternalLinkType](../../externallinktype/)
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


