---
title: "Enum ExternalLinkType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExternalLinkType enum. Dış bağlantı türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/externallinktype/
---
## ExternalLinkType enumeration

Harici bağlantı türünü temsil eder.

```csharp
public enum ExternalLinkType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| DDELink | `0` | DDE bağlantısını temsil eder. |
| External | `1` | Dış bağlantıyı temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkTypeDemo
    {
        public static void ExternalLinkTypeExample()
        {
            // Dış bağlantılar içeren bir dosya aç
            Workbook workbook = new Workbook("ExternalLinkTypeExample_original.xlsx");

            // Dış Bağlantıyı Al 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Dış bağlantının türünü göster
            Console.WriteLine("External Link Type: " + externalLink.Type);

            // Dış Bağlantının Veri Kaynağını Değiştir
            externalLink.DataSource = "d:\\link.xls";

            // Çalışma kitabını kaydedin
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }

    // Dış bağlantı türünü temsil eden enum
    public enum ExternalLinkType
    {
        DDELink = 0, // Represents the DDE link
        External = 1 // Represents external link
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


