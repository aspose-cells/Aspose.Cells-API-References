---
title: "Sınıf Border"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Border sınıfı. Hücre kenarlığını temsil eden nesneyi kapsüller"
type: docs
url: /tr/net/aspose.cells/border/
---
## Border class

Hücre kenarlığını temsil eden nesneyi kapsüller.

```csharp
public class Border
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ArgbColor](../../aspose.cells/border/argbcolor/) { get; set; } | 32-bit ARGB değeriyle rengi alır ve ayarlar. |
| [Color](../../aspose.cells/border/color/) { get; set; } | Kenarlığın rengini alır veya ayarlar. |
| [LineStyle](../../aspose.cells/border/linestyle/) { get; set; } | Hücre kenarlık tipini alır veya ayarlar. |
| [ThemeColor](../../aspose.cells/border/themecolor/) { get; set; } | Kenarlığın tema rengini alır ve ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderDemo
    {
        public static void BorderExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // Workbook nesnesine yeni bir çalışma sayfası ekleme
            workbook.Worksheets.Add();

            // Eklenen yeni çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasından "A1" hücresine erişme
            Cell cell = worksheet.Cells["A1"];

            // "A1" hücresine bir değer ekleme
            cell.PutValue("Hello World");

            // Hücre stilini alıyor
            Style style = cell.GetStyle();

            // Üst kenarlığın çizgi stilini ayarlama
            Border topBorder = style.Borders[BorderType.TopBorder];
            topBorder.LineStyle = CellBorderType.Medium;
            topBorder.Color = Color.Red;

            // Alt kenarlığın çizgi stilini ayarlama
            Border bottomBorder = style.Borders[BorderType.BottomBorder];
            bottomBorder.LineStyle = CellBorderType.Thick;
            bottomBorder.Color = Color.Blue;

            // Sol kenarlığın çizgi stilini ayarlama
            Border leftBorder = style.Borders[BorderType.LeftBorder];
            leftBorder.LineStyle = CellBorderType.Dashed;
            leftBorder.Color = Color.Green;

            // Sağ kenarlığın çizgi stilini ayarlama
            Border rightBorder = style.Borders[BorderType.RightBorder];
            rightBorder.LineStyle = CellBorderType.Dotted;
            rightBorder.Color = Color.Purple;

            // Stili hücreye uygulama
            cell.SetStyle(style);

            // Excel dosyasını kaydetme
            workbook.Save("BorderExample.xlsx");
            workbook.Save("BorderExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


