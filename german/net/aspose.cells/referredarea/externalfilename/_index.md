---
title: "ReferredArea.ExternalFileName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReferredArea-Eigenschaft. Den externen Dateinamen abrufen, wenn dies eine externe Referenz ist"
type: docs
url: /de/net/aspose.cells/referredarea/externalfilename/
---
## ReferredArea.ExternalFileName property

Den externen Dateinamen abrufen, wenn dies eine externe Referenz ist.

```csharp
public string ExternalFileName { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyExternalFileNameDemo
    {
        public static void Run()
        {
            // Eine Arbeitsmappe mit externer Referenz erstellen
            Workbook wb = new Workbook();
            
            // Einen Namen erstellen, der auf eine externe Arbeitsmappe verweist
            int index = wb.Worksheets.Names.Add("RefExternalName");
            wb.Worksheets.Names[index].RefersTo = "='[ExternalLinkSource.xlsx]Sheet1'!$A$1:$C$3";
            
            // Hole den referenzierten Bereich
            ReferredArea ra = wb.Worksheets.Names["RefExternalName"].GetReferredAreas(false)[0];
            
            // Demonstriere die ExternalFileName-Eigenschaft
            Console.WriteLine("External File Name: " + ra.ExternalFileName);
            Console.WriteLine("Sheet Name: " + ra.SheetName);
            Console.WriteLine("Area: R" + ra.StartRow + "C" + ra.StartColumn + 
                              " to R" + ra.EndRow + "C" + ra.EndColumn);
            
            // Überprüfe den externen Dateinamen
            if (!ra.ExternalFileName.EndsWith("ExternalLinkSource.xlsx"))
            {
                Console.WriteLine("Error: ExternalFileName should be ExternalLinkSource.xlsx");
            }
        }
    }
}
```

### Siehe auch

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


