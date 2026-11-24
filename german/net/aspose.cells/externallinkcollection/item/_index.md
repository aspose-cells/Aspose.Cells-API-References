---
title: "ExternalLinkCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalLinkCollection-Eigenschaft. Gibt das ExternalLink-Element am angegebenen Index zurück."
type: docs
url: /de/net/aspose.cells/externallinkcollection/item/
---
## ExternalLinkCollection indexer

Gibt das [`ExternalLink`](../../externallink/) Element am angegebenen Index zurück.

```csharp
public ExternalLink this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe mit Beispiel-externen Links
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige externe Links hinzu
            worksheet.Cells["A1"].Formula = "='C:\\Temp\\External1.xlsx'!A1";
            worksheet.Cells["A2"].Formula = "='C:\\Temp\\External2.xlsx'!B2";
            
            // Greife auf externe Links über die Item-Eigenschaft zu.
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

### Siehe auch

* class [ExternalLink](../../externallink/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


