---
title: "ExternalLink.IsReferred"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalLink-Eigenschaft. Gibt an, ob dieser externe Link von anderen referenziert wird"
type: docs
url: /de/net/aspose.cells/externallink/isreferred/
---
## ExternalLink.IsReferred property

Gibt an, ob dieser externe Link von anderen referenziert wird.

```csharp
public bool IsReferred { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsReferredDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe mit externem Link
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge eine externe Linkreferenz hinzu
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // Prüfe, ob der externe Link referenziert wird
            if (workbook.Worksheets.ExternalLinks.Count > 0)
            {
                bool isReferred = workbook.Worksheets.ExternalLinks[0].IsReferred;
                Console.WriteLine("Is external link referred: " + isReferred);
            }
        }
    }
}
```

### Siehe auch

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


