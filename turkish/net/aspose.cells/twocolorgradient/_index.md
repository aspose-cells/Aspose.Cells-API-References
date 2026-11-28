---
title: "Class TwoColorGradient"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.TwoColorGradient sınıfı. İki renk geçişini temsil eder"
type: docs
url: /tr/net/aspose.cells/twocolorgradient/
---
## TwoColorGradient class

İki renkli geçişi temsil eder.

```csharp
public class TwoColorGradient
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [TwoColorGradient](twocolorgradient/)(Color, Color, GradientStyleType, int) |  |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Color1](../../aspose.cells/twocolorgradient/color1/) { get; set; } | İlk geçiş rengini alır ve ayarlar. |
| [Color2](../../aspose.cells/twocolorgradient/color2/) { get; set; } | İkinci geçiş rengini alır ve ayarlar. |
| [GradientStyleType](../../aspose.cells/twocolorgradient/gradientstyletype/) { get; set; } | Geçiş gölgelendirme stilini alır ve ayarlar. |
| [Variant](../../aspose.cells/twocolorgradient/variant/) { get; set; } | Geçiş varyantını alır ve ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class CellsClassTwoColorGradientDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // TwoColorGradient'i yapıcı parametreleriyle başlat
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightSkyBlue, 
                Color.DarkBlue, 
                GradientStyleType.DiagonalUp, 
                2);

            // Başlatmadan sonra degrade özelliklerini değiştir
            gradient.GradientStyleType = GradientStyleType.DiagonalDown;

            // Hücre stilini oluştur ve degrade uygula
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);

            // Stili hücreye uygula ve içeriği ekle
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Aspose.Cells TwoColorGradient Demo");
            cell.SetStyle(style);

            // Görünürlük için hücre boyutlarını ayarla
            worksheet.Cells.SetRowHeight(1, 45);
            worksheet.Cells.SetColumnWidth(1, 55);

            // Sonucu degrade biçimlendirmesiyle kaydet
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


