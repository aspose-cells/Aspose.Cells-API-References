---
title: "Sınıf ThemeColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ThemeColor sınıfı. Bir tema rengini temsil eder"
type: docs
url: /tr/net/aspose.cells/themecolor/
---
## ThemeColor class

Bir tema rengini temsil eder.

```csharp
public class ThemeColor
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ThemeColor](themecolor/)(ThemeColorType, double) |  |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ColorType](../../aspose.cells/themecolor/colortype/) { get; set; } | Tema tipini alır ve ayarlar. |
| [Tint](../../aspose.cells/themecolor/tint/) { get; set; } | Renk tonu değerini alır ve ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorDemo
    {
        public static void ThemeColorExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // A1 hücresine değer ekleme
            cells["A1"].PutValue("Hello World");

            // A1 hücresinin stilini alma
            Style style = cells["A1"].GetStyle();

            // ThemeColorType.Text2 renk tipini %40 açık yaparak yazı tipi rengi olarak ayarla.
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
            style.Pattern = BackgroundType.Solid;

            // ThemeColorType.Background2 renk tipini %75 koyulaştırarak ön plan rengi olarak ayarla
            style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);

            // Stili A1 hücresine uygulama
            cells["A1"].SetStyle(style);

            // Excel dosyasını kaydetme
            workbook.Save("ThemeColorExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


