---
title: "CopyOptions.ExtendToAdjacentRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CopyOptions özelliği. Aralığı komşu bir aralığa kopyalarken aralıkların genişletilip genişletilmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/copyoptions/extendtoadjacentrange/
---
## CopyOptions.ExtendToAdjacentRange property

Aralığı bitişik aralığa kopyalarken aralıkların genişletilip genişletilmeyeceğini gösterir.

```csharp
public bool ExtendToAdjacentRange { get; set; }
```

### Açıklamalar

True ise, yalnızca köprü aralığını genişletir, komşu satırlara köprü kopyalarken yeni bir köprü eklemez.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyExtendToAdjacentRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // A1 hücresine bir köprü ekleyin
            ws.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Kopya seçeneklerini oluşturun ve ExtendToAdjacentRange özelliğini true olarak ayarlayın
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ExtendToAdjacentRange = true;

            // Kopya seçenekleriyle satır 0'ı satır 1'e kopyalayın
            ws.Cells.CopyRows(ws.Cells, 0, 1, 1, copyOptions);

            // Hyperlink'in bitişik aralığa genişletildiğini doğrulayın
            Console.WriteLine("Hyperlink count after copy: " + ws.Hyperlinks.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


