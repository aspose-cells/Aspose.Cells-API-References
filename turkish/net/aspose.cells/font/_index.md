---
title: "Sınıf Font"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Font sınıfı. Elektronik tablo içinde kullanılan yazı tipi nesnesini kapsüller"
type: docs
url: /tr/net/aspose.cells/font/
---
## Font class

Bir elektronik tabloda kullanılan yazı tipi nesnesini kapsüller.

```csharp
public class Font
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | 32-bit ARGB değeriyle rengi alır ve ayarlar. |
| [CapsType](../../aspose.cells/font/capstype/) { get; set; } | (**Obsolete.**) Metin büyük harf tipini alır ve ayarlar. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | Karakter kümesini temsil eder. |
| [Color](../../aspose.cells/font/color/) { get; set; } | Yazı tipinin Rengini alır veya ayarlar. |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | Yazı tipinin çift boyutunu alır ve ayarlar. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | Yazı tipinin kalın olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | Yazı tipinin italik olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [IsNormalizeHeights](../../aspose.cells/font/isnormalizeheights/) { get; set; } | (**Obsolete.**) Metin yürütmesine uygulanacak yükseklik normalizasyonunun olup olmadığını gösterir. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | Yazı tipinin tek çizgiyle üzeri çizili olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | Yazı tipinin alt simge olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | Yazı tipinin üst simge olup olmadığını gösteren bir değeri alır veya ayarlar. |
| virtual [Name](../../aspose.cells/font/name/) { get; set; } | `Font` adını alır veya ayarlar. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | Yazı tipinin şema türünü alır ve ayarlar. |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | Komut ofsetini yüzde biriminde alır ve ayarlar. |
| [Size](../../aspose.cells/font/size/) { get; set; } | Yazı tipinin boyutunu alır veya ayarlar. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | Metnin üzeri çizme tipini alır. |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | Tema rengini alır ve ayarlar. |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | Yazı tipinin alt çizgi tipini alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/#equals)(Font) | İki yazı tipinin eşit olup olmadığını denetler. |
| [SetName](../../aspose.cells/font/setname/)(string, FontSchemeType) | Yazı tipinin adını ve şemasını ayarlar. |
| override [ToString](../../aspose.cells/font/tostring/)() | Geçerli Cell nesnesini temsil eden bir dize döndürür. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontDemo
    {
        public static void FontExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // Eklenen yeni çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasından "A1" hücresine erişme
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // "A1" hücresine bir değer ekleme
            cell.PutValue("Hello Aspose!");

            // Hücre stilinin yazı tipi nesnesine erişim
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Yazı tipi adını "Times New Roman" olarak ayarlama
            font.Name = "Times New Roman";

            // Yazı tipi boyutunu 14 olarak ayarlama
            font.Size = 14;

            // Yazı tipi rengini Kırmızı olarak ayarlama
            font.Color = Color.Red;

            // Ek yazı tipi özelliklerini ayarlama
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;
            font.IsStrikeout = false;
            font.IsSuperscript = false;
            font.IsSubscript = false;
            font.Charset = 1;
            font.CapsType = TextCapsType.None;
            font.StrikeType = TextStrikeType.None;
            font.ScriptOffset = 0;
            font.DoubleSize = 14.0;
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            font.ArgbColor = Color.Red.ToArgb();
            font.IsNormalizeHeights = false;
            font.SchemeType = FontSchemeType.None;

            // Excel dosyasını kaydetme
            workbook.Save("FontExample.xlsx");
            workbook.Save("FontExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


