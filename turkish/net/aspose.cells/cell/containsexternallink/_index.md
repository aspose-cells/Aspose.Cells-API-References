---
title: "Cell.ContainsExternalLink"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Bu hücrenin harici bir bağlantı içerip içermediğini gösterir. Yalnızca hücre bir formül hücresi olduğunda geçerlidir."
type: docs
url: /tr/net/aspose.cells/cell/containsexternallink/
---
## Cell.ContainsExternalLink property

Bu hücrenin harici bir bağlantı içerip içermediğini gösterir. Yalnızca hücre bir formül hücresi olduğunda geçerlidir.

```csharp
public bool ContainsExternalLink { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyContainsExternalLinkDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Örnek veri ve harici bağlantı ekleyin
            sheet.Cells["A1"].PutValue("External Link:");
            sheet.Cells["B1"].Formula = "=HYPERLINK(\"https://www.aspose.com\", \"Aspose\")";
            
            // Hücrelerin harici bağlantı içerip içermediğini kontrol edin
            Console.WriteLine("A1 ContainsExternalLink: " + sheet.Cells["A1"].ContainsExternalLink);
            Console.WriteLine("B1 ContainsExternalLink: " + sheet.Cells["B1"].ContainsExternalLink);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


