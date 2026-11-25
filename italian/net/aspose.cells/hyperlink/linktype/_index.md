---
title: "Hyperlink.LinkType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Hyperlink. Ottiene il tipo di collegamento"
type: docs
url: /it/net/aspose.cells/hyperlink/linktype/
---
## Hyperlink.LinkType property

Ottiene il tipo di collegamento.

```csharp
public TargetModeType LinkType { get; }
```

### Esempi

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
            
            // Aggiungi un collegamento ipertestuale esterno
            int hyperlinkIndex = worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            Hyperlink link = worksheet.Hyperlinks[hyperlinkIndex];
            
            // Dimostra la proprietà LinkType
            Console.WriteLine("Hyperlink LinkType: " + link.LinkType);
            
            // Pulisci
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Vedi anche

* enum [TargetModeType](../../targetmodetype/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


