---
title: "Comment Sınıfı"
linktitle: "Comment"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Yorum sınıfı. Go'da yorumu temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/comment/
---

## Comment class

Bir hücre yorumunu temsil eden nesneyi kapsüller.

```go

type Comment struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetAuthor](./getauthor/) | Orijinal yorum yazarının Adını alır ve ayarlar |
| [SetAuthor](./setauthor/) | Orijinal yorum yazarının Adını alır ve ayarlar |
| [GetCommentShape](./getcommentshape/) | Belirtilen yoruma ekli şekli temsil eden bir Shape nesnesi al. |
| [GetRow](./getrow/) | Yorumun satır indeksini alır. |
| [GetColumn](./getcolumn/) | Yorumun sütun indeksini alır. |
| [IsThreadedComment](./isthreadedcomment/) | Bu yorumun bir zincirleme yorum olup olmadığını gösterir. |
| [GetThreadedComments](./getthreadedcomments/) | Zincirleme yorumların listesini alır; |
| [GetNote](./getnote/) | Yorumun içeriğini temsil eder. |
| [SetNote](./setnote/) | Yorumun içeriğini temsil eder. |
| [GetHtmlNote](./gethtmlnote/) | Bu yorumda veri ve bazı biçimleri içeren html dizesini alır ve ayarlar. |
| [SetHtmlNote](./sethtmlnote/) | Bu yorumda veri ve bazı biçimleri içeren html dizesini alır ve ayarlar. |
| [GetFont](./getfont/) | Yorumun yazı tipini alır. |
| [FormatCharacters](./formatcharacters/) | Bazı karakterleri yazı tipi ayarıyla biçimlendir. |
| [Characters](./characters/) | Yorum metni içinde bir karakter aralığını temsil eden bir Characters nesnesi döndürür. |
| [GetRichFormattings](./getrichformattings/) | Yorum metni içinde bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür. |
| [IsVisible](./isvisible/) | Yorumun görünür olup olmadığını temsil eder. |
| [SetIsVisible](./setisvisible/) | Yorumun görünür olup olmadığını temsil eder. |
| [GetTextOrientationType](./gettextorientationtype/) | Yorumun metin yönlendirme tipini alır ve ayarlar. |
| [SetTextOrientationType](./settextorientationtype/) | Yorumun metin yönlendirme tipini alır ve ayarlar. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Yorumun metin yatay hizalama tipini alır ve ayarlar. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Yorumun metin yatay hizalama tipini alır ve ayarlar. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Yorumun metin dikey hizalama tipini alır ve ayarlar. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Yorumun metin dikey hizalama tipini alır ve ayarlar. |
| [GetAutoSize](./getautosize/) | Yorumun boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir. Not: Bazı özel durumlarda (örneğin Mac ortamı) bu ayar etkili olmayabilir. Bu ayar etkili olmazsa, lütfen FitToTextSize() ile değiştirin. |
| [SetAutoSize](./setautosize/) | Yorumun boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir. Not: Bazı özel durumlarda (örneğin Mac ortamı) bu ayar etkili olmayabilir. Bu ayar etkili olmazsa, lütfen FitToTextSize() ile değiştirin. |
| [GetHeightCM](./getheightcm/) | Yorumun yüksekliğini santimetre biriminde temsil eder. |
| [SetHeightCM](./setheightcm/) | Yorumun yüksekliğini santimetre biriminde temsil eder. |
| [GetWidthCM](./getwidthcm/) | Yorumun genişliğini santimetre biriminde temsil eder. |
| [SetWidthCM](./setwidthcm/) | Yorumun genişliğini santimetre biriminde temsil eder. |
| [GetWidth](./getwidth/) | Yorumun genişliğini piksel biriminde temsil eder. |
| [SetWidth](./setwidth/) | Yorumun genişliğini piksel biriminde temsil eder. |
| [GetHeight](./getheight/) | Yorumun yüksekliğini piksel biriminde temsil eder. |
| [SetHeight](./setheight/) | Yorumun yüksekliğini piksel biriminde temsil eder. |
| [GetWidthInch](./getwidthinch/) | Yorumun genişliğini inç biriminde temsil eder. |
| [SetWidthInch](./setwidthinch/) | Yorumun genişliğini inç biriminde temsil eder. |
| [GetHeightInch](./getheightinch/) | Yorumun yüksekliğini inç biriminde temsil eder. |
| [SetHeightInch](./setheightinch/) | Yorumun yüksekliğini inç biriminde temsil eder. |
