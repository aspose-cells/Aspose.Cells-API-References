---
title: "Range.Hyperlinks"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Aralıktaki tüm köprüleri alır"
type: docs
url: /tr/net/aspose.cells/range/hyperlinks/
---
## Range.Hyperlinks property

Aralıktaki tüm köprüleri alır.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyHyperlinksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine bir köprü ekleyin
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // A1 içeren bir aralık oluşturun
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1");
            
            // Aralıktaki köprüleri alın
            Hyperlink[] hyperlinks = range.Hyperlinks;
            
            // Köprü bilgilerini gösterin
            if (hyperlinks.Length > 0)
            {
                Console.WriteLine("Hyperlink found:");
                Console.WriteLine($"Address: {hyperlinks[0].Address}");
                Console.WriteLine($"Link Type: {hyperlinks[0].LinkType}");
                
                // Köprüyü sil
                hyperlinks[0].Delete();
                Console.WriteLine("Hyperlink deleted");
            }
            
            // Bağlantının kaldırıldığını doğrulayın.
            Console.WriteLine($"Total hyperlinks in worksheet: {worksheet.Hyperlinks.Count}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


