---
title: "ExternalLink.PathType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalLink özelliği. Bu harici bağlantının yol türünü alır"
type: docs
url: /tr/net/aspose.cells/externallink/pathtype/
---
## ExternalLink.PathType property

Bu harici bağlantının yol türünü alın

```csharp
public string PathType { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyPathTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekle
            Worksheet sheet = workbook.Worksheets[0];
            
            // Başka bir çalışma kitabına harici bir bağlantı oluşturun
            sheet.Cells["A1"].Formula = "='C:\\Temp\\ExternalWorkbook.xlsx'!Sheet1!A1";
            
            // Harici bağlantıyı al
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // Harici bağlantının yol türünü göster
            Console.WriteLine("Path Type: " + externalLink.PathType);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ExternalLinkDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


