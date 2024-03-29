---
title: Comment
second_title: Aspose.Cells for .NET API Referansı
description: Bir hücre yorumunu temsil eden nesneyi kapsüller.
type: docs
weight: 1080
url: /tr/net/aspose.cells/comment/
---
## Comment class

Bir hücre yorumunu temsil eden nesneyi kapsüller.

```csharp
public class Comment
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Author](../../aspose.cells/comment/author) { get; set; } | Orijinal yorumun adını alır ve ayarlar Author |
| [AutoSize](../../aspose.cells/comment/autosize) { get; set; } | Yorum boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir. |
| [Column](../../aspose.cells/comment/column) { get; } | Yorumun sütun dizinini alır. |
| [CommentShape](../../aspose.cells/comment/commentshape) { get; } | Belirtilen açıklamaya eklenen şekli temsil eden bir Shape nesnesi alın. |
| [Font](../../aspose.cells/comment/font) { get; } | Yorumun yazı tipini alır. |
| [Height](../../aspose.cells/comment/height) { get; set; } | Piksel birimi cinsinden yorumun Yüksekliğini temsil eder. |
| [HeightCM](../../aspose.cells/comment/heightcm) { get; set; } | Yorumun yüksekliğini santimetre cinsinden temsil eder. |
| [HeightInch](../../aspose.cells/comment/heightinch) { get; set; } | Yorumun yüksekliğini inç cinsinden temsil eder. |
| [HtmlNote](../../aspose.cells/comment/htmlnote) { get; set; } | Bu yorumdaki verileri ve bazı biçimleri içeren html dizesini alır ve ayarlar. |
| [IsThreadedComment](../../aspose.cells/comment/isthreadedcomment) { get; } | Bu yorumun zincirlenmiş bir yorum olup olmadığını gösterir. |
| [IsVisible](../../aspose.cells/comment/isvisible) { get; set; } | Yorumun görünür olup olmadığını temsil eder. |
| [Note](../../aspose.cells/comment/note) { get; set; } | Yorumun içeriğini temsil eder. |
| [Row](../../aspose.cells/comment/row) { get; } | Yorumun satır dizinini alır. |
| [TextHorizontalAlignment](../../aspose.cells/comment/texthorizontalalignment) { get; set; } | Yorumun metin yatay hizalama türünü alır ve ayarlar. |
| [TextOrientationType](../../aspose.cells/comment/textorientationtype) { get; set; } | Yorumun metin yönlendirme türünü alır ve ayarlar. |
| [TextVerticalAlignment](../../aspose.cells/comment/textverticalalignment) { get; set; } | Yorumun metin dikey hizalama türünü alır ve ayarlar. |
| [ThreadedComments](../../aspose.cells/comment/threadedcomments) { get; } | Dizili yorumların listesini alır; |
| [Width](../../aspose.cells/comment/width) { get; set; } | Piksel birimi cinsinden yorumun genişliğini temsil eder. |
| [WidthCM](../../aspose.cells/comment/widthcm) { get; set; } | Yorumun genişliğini santimetre cinsinden temsil eder. |
| [WidthInch](../../aspose.cells/comment/widthinch) { get; set; } | Yorumun genişliğini inç cinsinden temsil eder. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Characters](../../aspose.cells/comment/characters)(int, int) | Yorum metni içinde bir dizi karakter temsil eden bir Karakterler nesnesi döndürür. |
| [FormatCharacters](../../aspose.cells/comment/formatcharacters)(int, int, Font, StyleFlag) | Bazı karakterleri yazı tipi ayarıyla biçimlendirin. |
| [GetCharacters](../../aspose.cells/comment/getcharacters)() | Yorum metninde bir dizi karakter temsil eden tüm Karakter nesnelerini döndürür. |

### Örnekler

```csharp
[C#]

Workbook workbook = new Workbook();
CommentCollection comments = workbook.Worksheets[0].Comments;

// A1 hücresine yorum ekle
int commentIndex1 = comments.Add(0, 0);
Comment comment1 = comments[commentIndex1];
comment1.Note = "First note.";
comment1.Font.Name = "Times New Roman";

// B2 hücresine yorum ekle
comments.Add("B2");
Comment comment2 = comments["B2"];
comment2.Note = "Second note.";

//işini yap

//Excel dosyasını kaydedin.
workbook.Save("exmaple.xlsx");

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim comments as CommentCollection = workbook.Worksheets(0).Comments
 
'A1 hücresine yorum ekle
Dim commentIndex1 as Integer = comments.Add(0, 0)
Dim comment1 as Comment = comments(commentIndex1)
comment1.Note = "First note."
comment1.Font.Name = "Times New Roman"

'B2 hücresine yorum ekle
comments.Add("B2")
Dim comment2 As Comment = comments("B2")
comment2.Note = "Second note."
 
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
