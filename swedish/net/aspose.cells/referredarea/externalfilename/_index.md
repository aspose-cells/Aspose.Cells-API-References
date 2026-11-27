---
title: "ReferredArea.ExternalFileName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReferredArea-egenskapen. Hämta det externa filnamnet om detta är en extern referens"
type: docs
url: /sv/net/aspose.cells/referredarea/externalfilename/
---
## ReferredArea.ExternalFileName property

Hämta det externa filnamnet om detta är en extern referens.

```csharp
public string ExternalFileName { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyExternalFileNameDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med extern referens
            Workbook wb = new Workbook();
            
            // Skapa ett namn som refererar till en extern arbetsbok
            int index = wb.Worksheets.Names.Add("RefExternalName");
            wb.Worksheets.Names[index].RefersTo = "='[ExternalLinkSource.xlsx]Sheet1'!$A$1:$C$3";
            
            // Hämta det refererade området
            ReferredArea ra = wb.Worksheets.Names["RefExternalName"].GetReferredAreas(false)[0];
            
            // Demonstrera ExternalFileName-egenskapen
            Console.WriteLine("External File Name: " + ra.ExternalFileName);
            Console.WriteLine("Sheet Name: " + ra.SheetName);
            Console.WriteLine("Area: R" + ra.StartRow + "C" + ra.StartColumn + 
                              " to R" + ra.EndRow + "C" + ra.EndColumn);
            
            // Verifiera det externa filnamnet
            if (!ra.ExternalFileName.EndsWith("ExternalLinkSource.xlsx"))
            {
                Console.WriteLine("Error: ExternalFileName should be ExternalLinkSource.xlsx");
            }
        }
    }
}
```

### Se även

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


