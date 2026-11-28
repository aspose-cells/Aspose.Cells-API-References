---
title: "Enum TextStrikeType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.TextStrikeType enum. Bu tip üstü çizgi tipini belirtir"
type: docs
url: /tr/net/aspose.cells/textstriketype/
---
## TextStrikeType enumeration

Bu tip, vurgu (üstü çizili) türünü belirtir.

```csharp
public enum TextStrikeType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Single | `0` | Metne tek bir üstü çizgi uygulanır. |
| Double | `1` | Metne çift üstü çizgi uygulanır. Yalnızca şekil veya grafik metinlerinde çalışır. |
| None | `2` | Metne üstü çizgi uygulanmaz. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextStrikeTypeDemo
    {
        public static void TextStrikeTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            // İlk çalışma sayfasının referansını alın.
            Worksheet worksheet = workbook.Worksheets[0];
            // Çalışma sayfasından "A1" hücresine erişme
            Cell cell = worksheet.Cells["A1"];
            // "A1" hücresine bir değer ekleme
            cell.PutValue("Hello Aspose!");

            // Hücrenin yazı tipine erişme
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Üstü çizgi tipini Tek olarak ayarlama
            font.StrikeType = TextStrikeType.Single;

            // Stili hücreye uygulayın
            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("TextStrikeTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


