---
title: "ExternalLink.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalLink özelliği. Harici bağlantının türünü alır"
type: docs
url: /tr/net/aspose.cells/externallink/type/
---
## ExternalLink.Type property

Harici bağlantının türünü alır.

```csharp
public ExternalLinkType Type { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekle
            Worksheet sheet = workbook.Worksheets[0];
            
            // Başka bir çalışma kitabına harici bir bağlantı oluşturun
            sheet.Cells["A1"].Formula = "='[link.xls]Sheet1'!A1";
            
            // Harici bağlantıyı al
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // Dış bağlantının türünü göster
            Console.WriteLine("External Link Type: " + externalLink.Type);
            
            // Harici bağlantının veri kaynağını değiştir
            externalLink.DataSource = "d:\\link.xls";
            
            // Çalışma kitabını kaydedin
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ExternalLinkType](../../externallinktype/)
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


