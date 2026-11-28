---
title: "Enum TextCapsType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.TextCapsType enum. Bu tip, metnin büyük harf tiplerini belirtir"
type: docs
url: /tr/net/aspose.cells/textcapstype/
---
## TextCapsType enumeration

Bu tip, metnin büyük harf türlerini belirtir.

```csharp
public enum TextCapsType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Kapak yok |
| All | `1` | Metne tüm büyük harfleri uygula. |
| Small | `2` | Metne küçük büyük harfleri uygula. |

### Açıklamalar

Yalnızca grafik ve şekle uygulanabilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextCapsTypeDemo
    {
        public static void TextCapsTypeExample()
        {
            // Örneğin, bir çalışma kitabı oluşturup kaydetmek için ek kod
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir hücrenin değerini ayarla
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello Aspose!");

            // Hücrenin stilini al
            Style style = cell.GetStyle();

            // Yazı tipi büyük harf tipini Tüm Büyük Harf olarak ayarla
            style.Font.CapsType = Aspose.Cells.TextCapsType.All;

            // Stili hücreye uygulayın
            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("TextCapsTypeExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


