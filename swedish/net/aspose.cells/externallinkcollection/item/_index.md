---
title: "ExternalLinkCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalLinkCollection-egenskap. Hämtar ExternalLink-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells/externallinkcollection/item/
---
## ExternalLinkCollection indexer

Hämtar [`ExternalLink`](../../externallink/) elementet på det angivna indexet.

```csharp
public ExternalLink this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempel på externa länkar
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till några externa länkar
            worksheet.Cells["A1"].Formula = "='C:\\Temp\\External1.xlsx'!A1";
            worksheet.Cells["A2"].Formula = "='C:\\Temp\\External2.xlsx'!B2";
            
            // Åtkomst till externa länkar med Item-egenskapen
            for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
            {
                ExternalLink link = workbook.Worksheets.ExternalLinks[i];
                Console.WriteLine($"External Link {i + 1}:");
                Console.WriteLine($"- DataSource: {link.DataSource}");
                Console.WriteLine($"- OriginalDataSource: {link.OriginalDataSource}");
            }
        }
    }
}
```

### Se även

* class [ExternalLink](../../externallink/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


