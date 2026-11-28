---
title: "PageSetup.GetHeader"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Bir Excel dosyasının üstbilgisini biçimlendiren bir betik alır"
type: docs
url: /tr/net/aspose.cells/pagesetup/getheader/
---
## PageSetup.GetHeader method

Excel dosyasının üst bilgisini biçimlendiren bir betiği alır.

```csharp
public string GetHeader(int section)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bölüm | Int32 | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bölüm 2 için üstbilgiyi ayarlayın
            worksheet.PageSetup.SetHeader(2, "&8Report ID: TEST01\n你好Public");
            
            // Bölüm 2 için üstbilgiyi al ve yazdır
            string header = worksheet.PageSetup.GetHeader(2);
            Console.WriteLine("Header for section 2: " + header);
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


