---
title: "HyperlinkCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HyperlinkCollection özelliği. Belirtilen indeksteki Hyperlink öğesini alır."
type: docs
url: /tr/net/aspose.cells/hyperlinkcollection/item/
---
## HyperlinkCollection indexer

Belirtilen indeksteki [`Hyperlink`](../../hyperlink/) öğesini alır.

```csharp
public Hyperlink this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

Belirtilen indeksteki öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine bir köprü ekleyin
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.example.com");
            
            // Item özelliğini kullanarak ilk bağlantıya erişin ve görüntü metnini ayarlayın.
            worksheet.Hyperlinks[0].TextToDisplay = "Click Here";
            
            // Bağlantı stilini ayarla (mavi altı çizili metin).
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.Underline = FontUnderlineType.Single;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Hyperlink](../../hyperlink/)
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


