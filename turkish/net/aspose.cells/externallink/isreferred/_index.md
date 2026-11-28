---
title: "ExternalLink.IsReferred"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalLink özelliği. Bu dış bağlantının başkaları tarafından referans alınıp alınmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/externallink/isreferred/
---
## ExternalLink.IsReferred property

Bu harici bağlantının diğerleri tarafından referans alınıp alınmadığını gösterir.

```csharp
public bool IsReferred { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsReferredDemo
    {
        public static void Run()
        {
            // Dış bağlantılı bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Dış bağlantı referansı ekleyin
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // Harici bağlantının başvurulup başvurulmadığını kontrol edin
            if (workbook.Worksheets.ExternalLinks.Count > 0)
            {
                bool isReferred = workbook.Worksheets.ExternalLinks[0].IsReferred;
                Console.WriteLine("Is external link referred: " + isReferred);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


