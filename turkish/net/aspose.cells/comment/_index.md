---
title: "Comment sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Comment sınıfı. Hücre yorumunu temsil eden nesneyi kapsüller."
type: docs
url: /tr/net/aspose.cells/comment/
---
## Comment class

Bir hücre yorumunu temsil eden nesneyi kapsüller.

```csharp
public class Comment
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Author](../../aspose.cells/comment/author/) { get; set; } | Orijinal yorum yazarının adını alır ve ayarlar. |
| [AutoSize](../../aspose.cells/comment/autosize/) { get; set; } | Yorumun boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir. Not: Bazı özel durumlarda (örneğin Mac ortamı) bu ayar etkili olmayabilir. Bu ayar etkili olmazsa, lütfen FitToTextSize() ile değiştirin. |
| [Column](../../aspose.cells/comment/column/) { get; } | Yorumun sütun indeksini alır. |
| [CommentShape](../../aspose.cells/comment/commentshape/) { get; } | Belirtilen yoruma ekli şekli temsil eden bir Shape nesnesi al. |
| [Font](../../aspose.cells/comment/font/) { get; } | Yorumun yazı tipini alır. |
| [Height](../../aspose.cells/comment/height/) { get; set; } | Yorumun yüksekliğini piksel biriminde temsil eder. |
| [HeightCM](../../aspose.cells/comment/heightcm/) { get; set; } | Yorumun yüksekliğini santimetre biriminde temsil eder. |
| [HeightInch](../../aspose.cells/comment/heightinch/) { get; set; } | Yorumun yüksekliğini inç biriminde temsil eder. |
| [HtmlNote](../../aspose.cells/comment/htmlnote/) { get; set; } | Bu yorumda veri ve bazı biçimleri içeren html dizesini alır ve ayarlar. |
| [IsThreadedComment](../../aspose.cells/comment/isthreadedcomment/) { get; } | Bu yorumun zincirli bir yorum olup olmadığını gösterir. |
| [IsVisible](../../aspose.cells/comment/isvisible/) { get; set; } | Yorumun görünür olup olmadığını temsil eder. |
| [Note](../../aspose.cells/comment/note/) { get; set; } | Yorumun içeriğini temsil eder. |
| [Row](../../aspose.cells/comment/row/) { get; } | Yorumun satır indeksini alır. |
| [TextHorizontalAlignment](../../aspose.cells/comment/texthorizontalalignment/) { get; set; } | Yorumun metin yatay hizalama tipini alır ve ayarlar. |
| [TextOrientationType](../../aspose.cells/comment/textorientationtype/) { get; set; } | Yorumun metin yönlendirme tipini alır ve ayarlar. |
| [TextVerticalAlignment](../../aspose.cells/comment/textverticalalignment/) { get; set; } | Yorumun metin dikey hizalama tipini alır ve ayarlar. |
| [ThreadedComments](../../aspose.cells/comment/threadedcomments/) { get; } | Zincirli yorumların listesini alır; |
| [Width](../../aspose.cells/comment/width/) { get; set; } | Yorumun genişliğini piksel biriminde temsil eder. |
| [WidthCM](../../aspose.cells/comment/widthcm/) { get; set; } | Yorumun genişliğini santimetre biriminde temsil eder. |
| [WidthInch](../../aspose.cells/comment/widthinch/) { get; set; } | Yorumun genişliğini inç biriminde temsil eder. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Characters](../../aspose.cells/comment/characters/)(int, int) | Yorum metni içindeki bir karakter aralığını temsil eden bir Characters nesnesi döndürür. |
| [FormatCharacters](../../aspose.cells/comment/formatcharacters/)(int, int, Font, StyleFlag) | Bazı karakterleri yazı tipi ayarıyla biçimlendir. |
| [GetRichFormattings](../../aspose.cells/comment/getrichformattings/)() | Yorum metni içindeki bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CommentDemo
    {
        public static void CommentExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            // Çalışma sayfasının yorumlar koleksiyonuna erişin
            CommentCollection comments = worksheet.Comments;

            // A1 hücresine bir yorum ekle
            int commentIndex1 = comments.Add(0, 0);
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Font.Name = "Times New Roman";
            comment1.Font.Size = 12;
            comment1.Font.Color = System.Drawing.Color.Red;
            comment1.Author = "Carl.Yang";
            comment1.HtmlNote = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            comment1.IsVisible = true;
            comment1.TextOrientationType = TextOrientationType.TopToBottom;
            comment1.TextHorizontalAlignment = TextAlignmentType.Center;
            comment1.TextVerticalAlignment = TextAlignmentType.Center;
            comment1.AutoSize = true;
            comment1.HeightCM = 1.0;
            comment1.WidthCM = 1.0;
            comment1.Width = 10;
            comment1.Height = 10;
            comment1.WidthInch = 1.0;
            comment1.HeightInch = 1.0;

            // Yorumun şekline erişin
            CommentShape shape = comment1.CommentShape;
            int w = shape.Width;
            int h = shape.Height;

            // B2 hücresine bir yorum ekleyin
            comments.Add("B2");
            Comment comment2 = comments["B2"];
            comment2.Note = "Second note.";

            // Çalışma kitabını kaydedin
            workbook.Save("CommentExample.xlsx");
            workbook.Save("CommentExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


