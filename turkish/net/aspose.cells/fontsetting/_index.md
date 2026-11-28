---
title: "Sınıf FontSetting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "**Aspose.Cells.FontSetting** sınıfı. Hücre metni içindeki bir karakter aralığını temsil eder"
type: docs
url: /tr/net/aspose.cells/fontsetting/
---
## FontSetting class

Hücre metni içindeki bir karakter aralığını temsil eder.

```csharp
public class FontSetting
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [FontSetting](fontsetting/)(int, int, WorksheetCollection) |  |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Bu nesnenin yazı tipini döndürür. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Karakterlerin uzunluğunu alır. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Karakterlerin başlangıç indeksini alır. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Metin seçeneklerini döndürür. |
| virtual [Type](../../aspose.cells/fontsetting/type/) { get; } | Metin düğümünün tipini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Önceden ayarlanmış WordArt stilini ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontSettingDemo
    {
        public static void FontSettingExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // Excel nesnesine yeni bir çalışma sayfası ekleme
            workbook.Worksheets.Add();

            // Eklenen yeni çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasından "A1" hücresine erişme
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // "A1" hücresine bir değer ekleme
            cell.PutValue("Visit Aspose!");

            // Karakter aralığını alma
            FontSetting character = cell.Characters(6, 7);

            // Seçili karakterlerin yazı tipini kalın olarak ayarlama
            character.Font.IsBold = true;

            // Seçili karakterlerin yazı tipi rengini mavi olarak ayarlama
            character.Font.Color = Color.Blue;

            // Excel dosyasını kaydetme
            workbook.Save("FontSettingExample.xlsx");
            workbook.Save("FontSettingExample.pdf");

        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


