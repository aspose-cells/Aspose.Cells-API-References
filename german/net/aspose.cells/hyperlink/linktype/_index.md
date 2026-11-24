---
title: "Hyperlink.LinkType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Hyperlink-Eigenschaft. Gibt den Linktyp zurück"
type: docs
url: /de/net/aspose.cells/hyperlink/linktype/
---
## Hyperlink.LinkType property

Ermittelt den Linktyp.

```csharp
public TargetModeType LinkType { get; }
```

### Beispiele

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
            
            // Externen Hyperlink hinzufügen
            int hyperlinkIndex = worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            Hyperlink link = worksheet.Hyperlinks[hyperlinkIndex];
            
            // LinkType-Eigenschaft demonstrieren
            Console.WriteLine("Hyperlink LinkType: " + link.LinkType);
            
            // Aufräumen
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Siehe auch

* enum [TargetModeType](../../targetmodetype/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


