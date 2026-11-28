---
title: "HyperlinkCollection.RemoveAt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HyperlinkCollection metodu. Bu koleksiyonda belirtilen indeksteki bağlantıyı kaldırın"
type: docs
url: /tr/net/aspose.cells/hyperlinkcollection/removeat/
---
## HyperlinkCollection.RemoveAt method

Bu koleksiyonda belirtilen indeksteki bağlantıyı kaldırın.

```csharp
public void RemoveAt(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Öğenin sıfır tabanlı indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // A1 hücresine bir köprü ekleyin
            sheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Kaldırmadan önce bağlantının mevcut olduğunu doğrulayın.
            Console.WriteLine("Hyperlinks count before removal: " + sheet.Hyperlinks.Count);
            
            // 0. indeksteki bağlantıyı kaldırın.
            sheet.Hyperlinks.RemoveAt(0);
            
            // Bağlantının kaldırıldığını doğrulayın.
            Console.WriteLine("Hyperlinks count after removal: " + sheet.Hyperlinks.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


