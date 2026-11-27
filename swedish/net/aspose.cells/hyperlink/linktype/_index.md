---
title: "Hyperlink.LinkType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Hyperlink‑egenskap. Hämtar länktypen"
type: docs
url: /sv/net/aspose.cells/hyperlink/linktype/
---
## Hyperlink.LinkType property

Hämtar länktypen.

```csharp
public TargetModeType LinkType { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyLinkTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en extern hyperlänk
            int hyperlinkIndex = worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            Hyperlink link = worksheet.Hyperlinks[hyperlinkIndex];
            
            // Demonstrera LinkType‑egenskapen
            Console.WriteLine("Hyperlink LinkType: " + link.LinkType);
            
            // Rensa upp
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Se även

* enum [TargetModeType](../../targetmodetype/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


