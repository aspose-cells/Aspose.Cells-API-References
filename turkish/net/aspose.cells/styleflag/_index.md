---
title: "StyleFlag sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.StyleFlag sınıfı. Uygulanan biçimlendirme özelliklerini gösteren bayrakları temsil eder."
type: docs
url: /tr/net/aspose.cells/styleflag/
---
## StyleFlag class

Uygulanan biçimlendirme özelliklerini gösteren bayrakları temsil eder.

```csharp
public class StyleFlag
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [StyleFlag](styleflag/)() | Tüm bayrakları false olarak ayarlayan bir nesne oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Alignments](../../aspose.cells/styleflag/alignments/) { get; set; } | Hizalama ayarı uygulanacak. |
| [All](../../aspose.cells/styleflag/all/) { get; set; } | Tüm özellikler uygulanacak. |
| [Borders](../../aspose.cells/styleflag/borders/) { get; set; } | Tüm kenar ayarları uygulanacak. |
| [BottomBorder](../../aspose.cells/styleflag/bottomborder/) { get; set; } | Alt kenar ayarları uygulanacak. |
| [CellShading](../../aspose.cells/styleflag/cellshading/) { get; set; } | Hücre gölgelendirme ayarı uygulanacak. |
| [DiagonalDownBorder](../../aspose.cells/styleflag/diagonaldownborder/) { get; set; } | Çapraz aşağı kenar ayarları uygulanacak. |
| [DiagonalUpBorder](../../aspose.cells/styleflag/diagonalupborder/) { get; set; } | Çapraz yukarı kenar ayarları uygulanacak. |
| [Font](../../aspose.cells/styleflag/font/) { get; set; } | Yazı tipi ayarları uygulanacak. |
| [FontBold](../../aspose.cells/styleflag/fontbold/) { get; set; } | Yazı tipi kalın ayarı uygulanacak. |
| [FontColor](../../aspose.cells/styleflag/fontcolor/) { get; set; } | Yazı tipi renk ayarı uygulanacak. |
| [FontItalic](../../aspose.cells/styleflag/fontitalic/) { get; set; } | Yazı tipi italik ayarı uygulanacak. |
| [FontName](../../aspose.cells/styleflag/fontname/) { get; set; } | Yazı tipi adı ayarı uygulanacak. |
| [FontScript](../../aspose.cells/styleflag/fontscript/) { get; set; } | Yazı tipi betik ayarı uygulanacak. |
| [FontSize](../../aspose.cells/styleflag/fontsize/) { get; set; } | Yazı tipi boyut ayarı uygulanacak. |
| [FontStrike](../../aspose.cells/styleflag/fontstrike/) { get; set; } | Yazı tipi üstü çizili ayarı uygulanacak. |
| [FontUnderline](../../aspose.cells/styleflag/fontunderline/) { get; set; } | Yazı tipi altı çizili ayarı uygulanacak. |
| [HideFormula](../../aspose.cells/styleflag/hideformula/) { get; set; } | Formülü gizle ayarı uygulanacak. |
| [HorizontalAlignment](../../aspose.cells/styleflag/horizontalalignment/) { get; set; } | Yatay hizalama ayarı uygulanacak. |
| [Indent](../../aspose.cells/styleflag/indent/) { get; set; } | Girinti seviyesi ayarı uygulanacak. |
| [LeftBorder](../../aspose.cells/styleflag/leftborder/) { get; set; } | Sol kenar ayarları uygulanacak. |
| [Locked](../../aspose.cells/styleflag/locked/) { get; set; } | Kilitli ayar uygulanacak. |
| [NumberFormat](../../aspose.cells/styleflag/numberformat/) { get; set; } | Sayı biçimi ayarı uygulanacak. |
| [QuotePrefix](../../aspose.cells/styleflag/quoteprefix/) { get; set; } | Formülü gizle ayarı uygulanacak. |
| [RightBorder](../../aspose.cells/styleflag/rightborder/) { get; set; } | Sağ kenar ayarları uygulanacak. |
| [Rotation](../../aspose.cells/styleflag/rotation/) { get; set; } | Döndürme ayarı uygulanacak. |
| [ShrinkToFit](../../aspose.cells/styleflag/shrinktofit/) { get; set; } | Sığdırmak için küçültme ayarı uygulanacak. |
| [TextDirection](../../aspose.cells/styleflag/textdirection/) { get; set; } | Metin yönü ayarı uygulanacak. |
| [TopBorder](../../aspose.cells/styleflag/topborder/) { get; set; } | Üst kenar ayarları uygulanacak. |
| [VerticalAlignment](../../aspose.cells/styleflag/verticalalignment/) { get; set; } | Dikey hizalama ayarı uygulanacak. |
| [WrapText](../../aspose.cells/styleflag/wraptext/) { get; set; } | Metni kaydırma ayarı uygulanacak. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagDemo
    {
        public static void StyleFlagExample()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı örnek veriler ekleyin
            worksheet.Cells["A1"].PutValue("Header 1");
            worksheet.Cells["B1"].PutValue("Header 2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Yeni bir stil nesnesi oluştur
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Yeni bir StyleFlag nesnesi oluştur
            StyleFlag styleFlag = new StyleFlag
            {
                All = true,
                Font = true,
                FontSize = true,
                FontBold = true,
                CellShading = true
            };

            // Stili bir hücre aralığına uygula
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B1");
            range.ApplyStyle(style, styleFlag);

            // Çalışma kitabını kaydedin
            workbook.Save("StyleFlagExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


