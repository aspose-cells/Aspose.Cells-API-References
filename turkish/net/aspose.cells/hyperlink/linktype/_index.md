---
title: "Hyperlink.LinkType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Hyperlink özelliği. Bağlantı tipini alır"
type: docs
url: /tr/net/aspose.cells/hyperlink/linktype/
---
## Hyperlink.LinkType property

Köprü tipini alır.

```csharp
public TargetModeType LinkType { get; }
```

### Örnekler

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
            
            // Harici bir köprü ekle
            int hyperlinkIndex = worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            Hyperlink link = worksheet.Hyperlinks[hyperlinkIndex];
            
            // LinkType özelliğini göster
            Console.WriteLine("Hyperlink LinkType: " + link.LinkType);
            
            // Temizle
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Ayrıca Bakınız

* enum [TargetModeType](../../targetmodetype/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


