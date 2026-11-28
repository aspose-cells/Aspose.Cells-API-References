---
title: "Sınıf TextParagraph"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Texts.TextParagraph sınıfı. Metin paragrafı ayarını temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textparagraph/
---
## TextParagraph class

Metin paragraf ayarının temsilidir.

```csharp
public class TextParagraph : FontSetting
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing.texts/textparagraph/alignmenttype/) { get; set; } | Paragrafın metin yatay hizalama türünü alır ve ayarlar. |
| [Bullet](../../aspose.cells.drawing.texts/textparagraph/bullet/) { get; } | Madde işaretini al. |
| [Children](../../aspose.cells.drawing.texts/textparagraph/children/) { get; } | Bu paragraftaki tüm metin akışlarını alır. Bu paragraf boşsa, paragrafı kendisini döndürür. |
| [DefaultTabSize](../../aspose.cells.drawing.texts/textparagraph/defaulttabsize/) { get; set; } | Bu paragraftaki sekme karakteri için varsayılan boyutu alır ve ayarlar. |
| [FirstLineIndent](../../aspose.cells.drawing.texts/textparagraph/firstlineindent/) { get; set; } | Paragraftaki metnin ilk satırına uygulanacak girinti boyutunu belirtir. |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Bu nesnenin yazı tipini döndürür (Miras alınan [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [FontAlignType](../../aspose.cells.drawing.texts/textparagraph/fontaligntype/) { get; set; } | Metin satırında kelimelerin dikey olarak nerede konumlandırıldığını belirler. Bu, karakterlerin temel çizgilere göre dikey yerleşimini kapsar. |
| [IsEastAsianLineBreak](../../aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/) { get; set; } | Bir Doğu Asya kelimesinin ikiye bölünüp tire eklenmeden bir sonraki satıra kaydırılıp kaydırılamayacağını belirtir. |
| [IsHangingPunctuation](../../aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/) { get; set; } | Noktalama işaretlerinin metin satırına zorla yerleştirilip yerleştirilmeyeceğini veya farklı bir satıra konulup konulmayacağını belirtir. |
| [IsLatinLineBreak](../../aspose.cells.drawing.texts/textparagraph/islatinlinebreak/) { get; set; } | Bir Latin kelimesinin ikiye bölünüp tire eklenmeden bir sonraki satıra kaydırılıp kaydırılamayacağını belirtir. |
| [LeftMargin](../../aspose.cells.drawing.texts/textparagraph/leftmargin/) { get; set; } | Paragrafın sol kenar boşluğunu belirtir. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Karakterlerin uzunluğunu alır (Miras alınan [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LineSpace](../../aspose.cells.drawing.texts/textparagraph/linespace/) { get; set; } | Paragrafta kullanılacak dikey boşluk miktarını alır ve ayarlar. |
| [LineSpaceSizeType](../../aspose.cells.drawing.texts/textparagraph/linespacesizetype/) { get; set; } | Paragrafta kullanılacak dikey boşluk miktarını alır ve ayarlar. |
| [RightMargin](../../aspose.cells.drawing.texts/textparagraph/rightmargin/) { get; set; } | Paragrafın sağ kenar boşluğunu belirtir. |
| [SpaceAfter](../../aspose.cells.drawing.texts/textparagraph/spaceafter/) { get; set; } | Bir paragraftan sonra bulunacak dikey boşluk miktarını alır ve ayarlar. |
| [SpaceAfterSizeType](../../aspose.cells.drawing.texts/textparagraph/spaceaftersizetype/) { get; set; } | Bir paragraftan sonra bulunacak dikey boşluk miktarını alır ve ayarlar. |
| [SpaceBefore](../../aspose.cells.drawing.texts/textparagraph/spacebefore/) { get; set; } | Bir paragraftan önce bulunacak dikey boşluk miktarını alır ve ayarlar. |
| [SpaceBeforeSizeType](../../aspose.cells.drawing.texts/textparagraph/spacebeforesizetype/) { get; set; } | Bir paragraftan önce bulunacak dikey boşluk miktarını alır ve ayarlar. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Karakterlerin başlangıç indeksini alır (Miras alınan [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Stops](../../aspose.cells.drawing.texts/textparagraph/stops/) { get; } | Sekme durakları listesini alır. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Metin seçeneklerini döndürür (Miras alınan [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.texts/textparagraph/type/) { get; } | Metin düğümünün tipini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Önceden ayarlanmış WordArt stilini ayarlar. (Şuradan devralınmıştır [`FontSetting`](../../aspose.cells/fontsetting/).) |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextParagraphDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            int textBoxIndex = sheet.TextBoxes.Add(10, 10, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = sheet.TextBoxes[textBoxIndex];
            
            // Birden fazla paragraf içeren metin içeriğini ayarla
            textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";

            // Metin paragraflarına eriş ve değiştir
            foreach (TextParagraph paragraph in textBox.TextBody.TextParagraphs)
            {
                // Paragraf özelliklerini ayarla
                paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
                paragraph.LineSpace = 20;
                paragraph.AlignmentType = TextAlignmentType.Center;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("TextParagraphDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


