---
title: "Enum TargetModeType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.TargetModeType enum. Hedef modunun türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/targetmodetype/
---
## TargetModeType enumeration

Hedef modunun türünü temsil eder.

```csharp
public enum TargetModeType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| External | `0` | Harici bağlantı |
| FilePath | `1` | Dosya veya klasörlerin yerel ve tam yolları. |
| Email | `2` | E-posta. |
| CellReference | `3` | Hücre veya adlandırılmış aralık üzerindeki bağlantı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTargetModeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Harici bir köprü ekle
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Köprüyü al ve TargetModeType değerini kontrol et
            Hyperlink link = worksheet.Hyperlinks[0];
            Console.WriteLine("Hyperlink TargetModeType: " + link.LinkType);
            
            // Köprüyü sil
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


