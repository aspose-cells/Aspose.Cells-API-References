---
title: "Range.AddHyperlink"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Belirtilen bir hücreye veya hücre aralığına bir hiperlink ekler."
type: docs
url: /tr/net/aspose.cells/range/addhyperlink/
---
## Range.AddHyperlink method

Belirtilen bir hücreye veya hücre aralığına bir hyperlink ekler.

```csharp
public Hyperlink AddHyperlink(string address, string textToDisplay, string screenTip)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| address | String | Köprünün adresi. |
| textToDisplay | String | Belirtilen köprü için görüntülenecek metin. |
| screenTip | String | Belirtilen bağlantı için screenTip metni. |

### Dönüş Değeri

[`Hyperlink`](../../hyperlink/) object.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodAddHyperlinkWithStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:A5");
            
            // Adres, görüntülenecek metin ve ekran ipucu ile bir hiperlink ekle.
            range.AddHyperlink("https://www.aspose.com", "Visit Aspose", "Click to go to Aspose website");
            
            // Çalışma kitabını kaydedin
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


