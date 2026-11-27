---
title: "ExternalLink.IsReferred"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalLink-egenskap. Anger om denna externa länk refereras av andra"
type: docs
url: /sv/net/aspose.cells/externallink/isreferred/
---
## ExternalLink.IsReferred property

Indikerar om denna externa länk refereras av andra.

```csharp
public bool IsReferred { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsReferredDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med extern länk
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till referens för extern länk
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // Kontrollera om den externa länken är refererad
            if (workbook.Worksheets.ExternalLinks.Count > 0)
            {
                bool isReferred = workbook.Worksheets.ExternalLinks[0].IsReferred;
                Console.WriteLine("Is external link referred: " + isReferred);
            }
        }
    }
}
```

### Se även

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


