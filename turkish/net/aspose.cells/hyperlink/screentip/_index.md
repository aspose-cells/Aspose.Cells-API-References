---
title: "Hyperlink.ScreenTip"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Hyperlink özelliği. Belirtilen köprü için ScreenTip metnini döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells/hyperlink/screentip/
---
## Hyperlink.ScreenTip property

Belirtilen köprü için ScreenTip metnini döndürür veya ayarlar.

```csharp
public string ScreenTip { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyScreenTipDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Click this hyperlink:");

            // ScreenTip ile bir köprü oluşturun
            int hLinkIdx = worksheet.Hyperlinks.Add("B1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks[hLinkIdx].ScreenTip = "Visit Aspose website for more information";

            // Çalışma kitabını kaydedin
            workbook.Save("HyperlinkWithScreenTip.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


