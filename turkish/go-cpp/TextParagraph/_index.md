---
title: "TextParagraph Sınıfı"
linktitle: "TextParagraph"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "TextParagraph sınıfı. Go dilinde metin paragrafını temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/textparagraph/
---

## TextParagraph class

Metin paragraf ayarını temsil eder.

```go

type TextParagraph struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewTextParagraph](./newtextparagraph/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetBullet](./getbullet/) | Madde işaretini alır. |
| [GetType](./gettype/) | Metin düğümünün tipini alır. |
| [GetLineSpaceSizeType](./getlinespacesizetype/) | Bir paragraf içinde kullanılacak dikey boşluk miktarını alır ve ayarlar. |
| [SetLineSpaceSizeType](./setlinespacesizetype/) | Bir paragraf içinde kullanılacak dikey boşluk miktarını alır ve ayarlar. |
| [GetLineSpace](./getlinespace/) | Bir paragraf içinde kullanılacak dikey boşluk miktarını alır ve ayarlar. |
| [SetLineSpace](./setlinespace/) | Bir paragraf içinde kullanılacak dikey boşluk miktarını alır ve ayarlar. |
| [GetSpaceAfterSizeType](./getspaceaftersizetype/) | Bir paragraftan sonra bulunacak dikey boşluk miktarını alır ve ayarlar. |
| [SetSpaceAfterSizeType](./setspaceaftersizetype/) | Bir paragraftan sonra bulunacak dikey boşluk miktarını alır ve ayarlar. |
| [GetSpaceAfter](./getspaceafter/) | Bir paragraftan sonra bulunacak dikey boşluk miktarını alır ve ayarlar. |
| [SetSpaceAfter](./setspaceafter/) | Bir paragraftan sonra bulunacak dikey boşluk miktarını alır ve ayarlar. |
| [GetSpaceBeforeSizeType](./getspacebeforesizetype/) | Bir paragraftan önce bulunacak dikey boşluk miktarını alır ve ayarlar. |
| [SetSpaceBeforeSizeType](./setspacebeforesizetype/) | Bir paragraftan önce bulunacak dikey boşluk miktarını alır ve ayarlar. |
| [GetSpaceBefore](./getspacebefore/) | Bir paragraftan önce bulunacak dikey boşluk miktarını alır ve ayarlar. |
| [SetSpaceBefore](./setspacebefore/) | Bir paragraftan önce bulunacak dikey boşluk miktarını alır ve ayarlar. |
| [GetStops](./getstops/) | Sekme durak listesi alır. |
| [IsLatinLineBreak](./islatinlinebreak/) | Bir Latin kelimesinin tire eklenmeden ikiye bölünüp bir sonraki satıra kaydırılıp kaydırılamayacağını belirtir. |
| [SetIsLatinLineBreak](./setislatinlinebreak/) | Bir Latin kelimesinin tire eklenmeden ikiye bölünüp bir sonraki satıra kaydırılıp kaydırılamayacağını belirtir. |
| [IsEastAsianLineBreak](./iseastasianlinebreak/) | Bir Doğu Asya kelimesinin tire eklenmeden ikiye bölünüp bir sonraki satıra kaydırılıp kaydırılamayacağını belirtir. |
| [SetIsEastAsianLineBreak](./setiseastasianlinebreak/) | Bir Doğu Asya kelimesinin tire eklenmeden ikiye bölünüp bir sonraki satıra kaydırılıp kaydırılamayacağını belirtir. |
| [IsHangingPunctuation](./ishangingpunctuation/) | Noktalama işaretlerinin metin satırına zorla yerleştirilip yerleştirilmeyeceğini veya farklı bir satıra konulup konulmayacağını belirtir. |
| [SetIsHangingPunctuation](./setishangingpunctuation/) | Noktalama işaretlerinin metin satırına zorla yerleştirilip yerleştirilmeyeceğini veya farklı bir satıra konulup konulmayacağını belirtir. |
| [GetRightMargin](./getrightmargin/) | Paragrafın sağ kenar boşluğunu belirtir. |
| [SetRightMargin](./setrightmargin/) | Paragrafın sağ kenar boşluğunu belirtir. |
| [GetLeftMargin](./getleftmargin/) | Paragrafın sol kenar boşluğunu belirtir. |
| [SetLeftMargin](./setleftmargin/) | Paragrafın sol kenar boşluğunu belirtir. |
| [GetFirstLineIndent](./getfirstlineindent/) | Paragraftaki metnin ilk satırına uygulanacak girinti boyutunu belirtir. |
| [SetFirstLineIndent](./setfirstlineindent/) | Paragraftaki metnin ilk satırına uygulanacak girinti boyutunu belirtir. |
| [GetFontAlignType](./getfontaligntype/) | Metin satırında kelimelerin dikey olarak nerede konumlandırıldığını belirler. Bu, karakterlerin temel çizgilere göre dikey yerleşimini ele alır. |
| [SetFontAlignType](./setfontaligntype/) | Metin satırında kelimelerin dikey olarak nerede konumlandırıldığını belirler. Bu, karakterlerin temel çizgilere göre dikey yerleşimini ele alır. |
| [GetAlignmentType](./getalignmenttype/) | Paragrafın metin yatay hizalama türünü alır ve ayarlar. |
| [SetAlignmentType](./setalignmenttype/) | Paragrafın metin yatay hizalama türünü alır ve ayarlar. |
| [GetDefaultTabSize](./getdefaulttabsize/) | Bu paragraftaki sekme karakterinin varsayılan boyutunu alır ve ayarlar. |
| [SetDefaultTabSize](./setdefaulttabsize/) | Bu paragraftaki sekme karakterinin varsayılan boyutunu alır ve ayarlar. |
| [GetChildren](./getchildren/) | Bu paragraftaki tüm metin akışlarını alır. Eğer bu paragraf boşsa, paragrafı kendisini döndürür. |
| [GetStartIndex](./getstartindex/) | Karakterlerin başlangıç indeksini alır. |
| [GetLength](./getlength/) | Karakterlerin uzunluğunu alır. |
| [GetFont](./getfont/) | Bu nesnenin yazı tipini döndürür. |
| [SetWordArtStyle](./setwordartstyle/) | Önceden ayarlanmış WordArt stilini ayarlar. |
| [GetTextOptions](./gettextoptions/) | Metin seçeneklerini döndürür. |
