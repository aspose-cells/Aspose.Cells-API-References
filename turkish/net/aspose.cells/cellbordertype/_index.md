---
title: "CellBorderType Enum"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CellBorderType enum. Hücre kenarlık tiplerini sıralar"
type: docs
url: /tr/net/aspose.cells/cellbordertype/
---
## CellBorderType enumeration

Bir hücrenin kenarlık türünü listeler.

```csharp
public enum CellBorderType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| DashDot | `9` | İnce tire-noktalı çizgiyi temsil eder. |
| DashDotDot | `11` | İnce tire-nokta-tire çizgiyi temsil eder. |
| Dashed | `3` | Kesikli çizgiyi temsil eder. |
| Dotted | `4` | Noktalı çizgiyi temsil eder. |
| Double | `6` | Çift çizgiyi temsil eder. |
| Hair | `7` | İnce çizgiyi temsil eder. |
| MediumDashDot | `10` | Orta kalınlıkta tire-noktalı çizgiyi temsil eder. |
| MediumDashDotDot | `12` | Orta kalınlıkta tire-nokta-tire çizgiyi temsil eder. |
| MediumDashed | `8` | Orta kalınlıkta kesikli çizgiyi temsil eder. |
| None | `0` | Çizgi olmadığını temsil eder. |
| Medium | `2` | Orta kalınlıkta çizgiyi temsil eder. |
| SlantedDashDot | `13` | Eğimli orta kalınlıkta tire-noktalı çizgiyi temsil eder. |
| Thick | `5` | Kalın çizgiyi temsil eder. |
| Thin | `1` | İnce çizgiyi temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellBorderTypeDemo
    {
        public static void CellBorderTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir aralık oluştur (A1:D4)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "D4");

            // Aralığın stilini al
            Style style = workbook.CreateStyle();

            // Aralık için farklı kenarlık stilleri ayarla
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = Color.Black;

            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;

            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.LeftBorder].Color = Color.Green;

            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
            style.Borders[BorderType.RightBorder].Color = Color.Red;

            // Stili aralığa uygula
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;
            range.ApplyStyle(style, styleFlag);

            // Çalışma kitabını kaydedin
            workbook.Save("CellBorderTypeExample.xlsx");
            workbook.Save("CellBorderTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


