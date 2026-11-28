---
title: "Enum BorderType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.BorderType enum. Kenar çizgisi ve diyagonal çizgi türlerini sıralar."
type: docs
url: /tr/net/aspose.cells/bordertype/
---
## BorderType enumeration

Kenarlık çizgisi ve diyagonal çizgi türlerini listeler.

```csharp
[Flags]
public enum BorderType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| LeftBorder | `1` | Sol kenar çizgisini temsil eder. |
| RightBorder | `2` | Sağ kenar çizgisinin var olduğunu temsil eder. |
| TopBorder | `4` | Üst kenar çizgisini temsil eder. |
| BottomBorder | `8` | Alt kenar çizgisini temsil eder. |
| DiagonalDown | `10` | Üst sol köşeden sağ alt köşeye doğru diyagonal çizgiyi temsil eder. |
| DiagonalUp | `20` | Alt sol köşeden sağ üst köşeye doğru diyagonal çizgiyi temsil eder. |
| Vertical | `40` | Yalnızca koşullu biçimlendirme, pivot tablo gibi dinamik stiller için. |
| Horizontal | `80` | Yalnızca koşullu biçimlendirme, pivot tablo gibi dinamik stiller için. |
| SideBorders | `F` | Dört kenar kenarını gösterir: LeftBorder, RightBorder, TopBorder ve BottomBorder. |
| Diagonal | `30` | Bazı API'ler için kullanıcının kolaylığı amacıyla birden fazla kenarın özel birleşimi. DiagonalUp ve DiagonalDown diyagonal kenarlarını gösterir. |
| DynamicStyleBorders | `C0` | Dinamik stilin Dikey ve Yatay yönlerini gösterir. |
| None | `0` | Hiçbir kenar belirtilmemiştir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderTypeDemo
    {
        public static void BorderTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            // Bir hücre aralığı oluşturun
            var range = worksheet.Cells.CreateRange("A1:D4");

            // Bir stil nesnesi oluşturun
            Style style = workbook.CreateStyle();
            // Aralık için kenarları ayarlayın
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);

            // Stili aralığa uygula
            StyleFlag flag = new StyleFlag { Borders = true };
            range.ApplyStyle(style, flag);

            // Çalışma kitabını kaydedin
            workbook.Save("BorderTypeExample.xlsx");
            workbook.Save("BorderTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


